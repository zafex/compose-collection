Generate private key
```shell
openssl genrsa -out private.pem -aes256 4096
```

Generate public key based on private key
```shell
openssl rsa -pubout -in private.pem -out public.pem
```
pass phrase: viloveul (atau ganti dan sesuaikan pada file docker-compose.yml) 

Run compose
```shell
docker-compose up
```

Tunggu beberapa saat (kira2 1 jam lah yak wkwkwk)

setelah selesai, aplikasi siap di port 19910 - 19913

| PORT | KETERANGAN |
| - | - |
| 19911 | Rest API (yang penting sih ini) |
| 19912 | Dashboard (Management, UI) |
| 19913 | Front/Theming/Display |

