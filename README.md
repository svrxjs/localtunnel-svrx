# localtunnel-svrx

Custom [localtunnel](https://github.com/localtunnel/localtunnel) server for [Svrx](https://github.com/svrxjs/svrx-plugin-localtunnel).

## How to use

```bash
npm install -g @svrx/cli
```

```bash
svrx -p "localtunnel?host=https://tunnel.svrx.io"
```

## How to deploy

 - Install [acme.sh](https://github.com/acmesh-official/acme.sh#1-how-to-install), [Docker](https://docs.docker.com/engine/install/), [docker-compose](https://docs.docker.com/compose/install/)

 - [Setup DNS API](https://github.com/acmesh-official/acme.sh/wiki/dnsapi)

 - Generate SSLs

```bash
./gen_ssl.sh -d tunnel.svrx.io --dns dns_cf
```

 - Run

 ```
 docker-compose up -d
 ```