## INSTALAÇÃO O11 DRM💻
Requisitos:

VPS BRASILEIRA COM 8GB E 4CORES NO MINIMO COM UBUNTU 20

Acesse sua maquina através do ssh e siga o passo a passo


1. Instalar o Docker:
```bash
sudo apt install docker.io
```

2. Agora copia e cola estes comandos, um por vez:
```bash
docker pull cyberpoison/o11-ott-streamer:latest
```
```bash
docker run \
  --name o11 \
  --restart always \
  --detach \
  --publish 1234:1234 \
  --volume /mnt/o11-ott:/mnt \
  cyberpoison/o11-ott-streamer:latest 
```
3. Após instalado, acesse o navegador com seu ip e porta 1234

   Ex.: http://186.200.120.44:1234

## SUPORTE E SCRIPTS 📎
Precisa de Scripts? Temos dos streaming:

Globoplay

SKY+

PlayPlus(Record)

Youtube

☎️ Contato: https://t.me/felipeadmin
