## INSTALL ZERO11
VPS PRECISA SER UBUNTU 18 OU 20

## INSTALAÇÃO
1. Baixe a imagem com o comando:
```bash
docker pull cyberpoison/o11-ott-streamer
```

2. Agora roda copia e cola isto:
```bash
docker run \
  --name o11 \
  --restart always \
  --detach \
  --publish 1234:1234 \
  --volume /mnt/o11-ott:/mnt \
  cyberpoison/o11-ott-streamer:latest 
```
