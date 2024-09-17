## INSTALL ZERO11
VPS PRECISA SER UBUNTU 18 OU 20

## INSTALAÇÃO
1. Instalar o Docker e baixar a imagem:
```bash
sudo apt install docker.io
```
```bash
docker pull cyberpoison/o11-ott-streamer:latest
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
