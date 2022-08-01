# coredns-doh-docker-compose
A docker-compose project for a DoH server using CoreDNS.

## Usage
0. Download this Repo, `cd` into it.
1. Get https certificate using [acme.sh](https://github.com/acmesh-official/acme.sh) for your domain, place `fullchain.pem` `key.pem` `ca.pem` into `./config` directory.
2. Run `docker-compose up -d` to start DoH server, you can use `docker-compose logs -f` to inspect logs and errors.
3. Use [doh](https://github.com/curl/doh) to test the started DoH server.
4. More info please check this [cn-version blog post](https://www.wogong.net/blog/2022/07/doh).
