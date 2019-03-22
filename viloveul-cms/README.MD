Generate private key
```shell
openssl genrsa -out private.pem -aes256 4096
```

Generate public key based on private key
```shell
openssl rsa -pubout -in private.pem -out public.pem
```

Run compose
```shell
docker-compose up
```