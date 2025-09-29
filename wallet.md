

### Tablo (main)

| Alan Adı | Veri Tipi | Açıklama |
|----------|-----------|----------|
| key | BLOB PRIMARY KEY | Birincil anahtar |
| value | BLOB | Değer |

## Cüzdan Tanımlayıcıları ve Adres Türleri

| Tanımlayıcı Tipi | Adres Formatı | Türetme Yolu | Checksum |
|------------------|--------------|--------------|----------|
| walletdescriptor | tr (Taproot) | /86h/0h/0h/0/* | #ghg3wrl4# |
| walletdescriptor | wpkh (SegWit) | /84h/0h/0h/0/* | #8ra0jm30# |
| walletdescriptor | sh(wpkh) (Nested SegWit) | /49h/0h/0h/0/* | #ym4n9wdl# |
| walletdescriptor | pkh (Legacy) | /44h/0h/0h/0/* | #uemxtkht# |
| walletdescriptorE | tr (Taproot) | /86h/0h/0h/1/* | #erdsnk0d$ |
| walletdescriptor | wpkh (SegWit) | /84h/0h/0h/1/* | #khcw0wph$ |
| walletdescriptor | sh(wpkh) (Nested SegWit) | /49h/0h/0h/1/* | #zcak7rxt$ |
| walletdescriptor | pkh (Legacy) | /44h/0h/0h/1/* | #dd78kr8n$ |

## İç ve Dış Adresler

| Anahtar Tipi | Değer | Kullanım |
|--------------|-------|----------|
| activeexternalspk | b4e64918193afd87fbfda7572fa4f5d0d7c093eab9cc4c61adc6fc076b0d0fbb | Dış adresler için aktif anahtarlar (ödeme alma) |
| activeinternalspk | b2bc9c60256aa139f22d801f97632a31a687f4838112de99c26c746797ee1e8b | İç adresler için aktif anahtarlar (para üstü) |
| activeexternalspkN | 4ebb1f890d344e082d7b20c771b3a3ab6051eb0088065653ff7a0ec975c77ebd0 | SegWit dış adresler için aktif anahtarlar |
| activeinternalspkE | 45cdad26c7dce0e9caa3330e06aa9e808d6b71198a8ed7b84939c64de6c6ee91 | Taproot iç adresler için aktif anahtarlar |
| activeexternalspk~P=w | 897e503d77ecc1ed478bb250ab4e6a64b11fdb853310f2d5afe8626cb2d4fe | Nested SegWit dış adresler için aktif anahtarlar |
| activeexternalspk | 080e4eb8b8ad9b3fb3bfcdc8e2a4478f40b8faf1c5788072457d4aea5328be2 | Legacy dış adresler için aktif anahtarlar |

## Cüzdan Önbellekleri (walletdescriptorcache)

| Önbellek Tipi | Değer | İlişkili Adres Türü |
|---------------|-------|---------------------|
| walletdescriptorcache | 00000000004a04169aad22000000000cf9f2b6258cd72565... | Taproot (tr) |
| walletdescriptorcacheN | 00000000004a040172afc90000000000... | SegWit (wpkh) |
| walletdescriptorcache~P=w | 00000000004a0454730d530000000000... | Nested SegWit (sh(wpkh)) |
| walletdescriptorcache | 00000000004a04fdfbee7800000000... | Legacy (pkh) |
| walletdescriptorcacheE | 00000000004a04169aad2200000001a9f2a1cfb508135a... | Taproot İç Adresler |

## Şifreleme Anahtarları (walletdescriptorckey)

| Anahtar Tipi | Değer | İlişkili Adres Türü |
|--------------|-------|---------------------|
| walletdescriptorckey | 21023c4462d7705ed6f282977767965... | Taproot (tr) |
| walletdescriptorckeyN | 21023c4462d7705ed6f282977767965... | SegWit (wpkh) |
| walletdescriptorckey~P=w | 21023c4462d7705ed6f282977767965... | Nested SegWit (sh(wpkh)) |
| walletdescriptorckey | 21023c4462d7705ed6f282977767965... | Legacy (pkh) |
| walletdescriptorckeyE | 21023c4462d7705ed6f282977767965... | Taproot İç Adresler |

## Yerel Hash Önbellekleri (walletdescriptorlhcache)

| Önbellek Tipi | Değer | İlişkili Adres Türü |
|---------------|-------|---------------------|
| walletdescriptorlhcache | 00000000004a03de2f239e80000000538a1037193d3b98... | Taproot (tr) |
| walletdescriptorlhcacheN | 00000000004a03eacc0763800000096acd906fea8i6... | SegWit (wpkh) |
| walletdescriptorlhcache~P=w | 00000000004a03651f76b68000000049997... | Nested SegWit (sh(wpkh)) |
| walletdescriptorlhcache | 00000000004a03e3d067988000000... | Legacy (pkh) |
| walletdescriptorlhcacheE | 00000000004a03de2f239e80000000538a1037... | Taproot İç Adresler |

## Blok Zinciri

Cüzdan dosyası, blok zincirinin durumunu takip etmek için çeşitli bilgiler içerir.

| Bilgi Tipi | Değer | Açıklama |
|------------|-------|----------|
| bestblock | 80110100001e2e4dd0e29bcf248a98fe0745ac6269547e... | En son bilinen blok hash'i |
| bestblock_nomerkle | 80110100001e2e4dd0e29bcf248a98fe0745ac... | Merkle kökü olmadan en son blok hash'i |
| minversion | ac970200 | Minimum cüzdan sürümü (2.97) |
| version | 24460400 | Cüzdan sürümü (4.46) |
| flags | 04000000 | Cüzdan bayrakları |
| mkey | 30ae0a82f32101a31b16a2a29a36a234af9490e6ac14d0ccfb45c532b8f0354cc8fadc7f28addf9deb7e24562af5dcdb5e08cf2ce9ececefbc | Ana şifreleme anahtarı |

## Extended Public Key (xpub)

```
xpub661MyMwAqRbcGqYqNCVeGV3hq9tE7uEz1mZtigrpvynka5bMpcaiXXmqrkSrnrm1dtnb4rLyKdcQxzipDPE4UVD8F6Hh7LmqC3nvSiupBET
```

