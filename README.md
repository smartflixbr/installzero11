# INSTALAÇÃO O11 DRM💻
#### Requisitos:

VPS BRASILEIRA COM NO MINIMO 8GB E 4CORES. Alem de Ubuntu 18 ou 20.

#### Acesse sua maquina através do ssh e siga o passo a passo:

### Instalar as atualizações e dependencias, faça um de cada vez:
```bash
sudo apt update && sudo apt upgrade -y
```
```bash
sudo apt install -y apache2
```
```bash
sudo apt install -y php7.4 libapache2-mod-php7.4 php7.4-sqlite3 php7.4-mysql php7.4-curl php7.4-json php7.4-cgi php7.4-xml
```
```bash
sudo apt install -y ffmpeg
```
```bash
sudo service apache2 restart
```

### Instalar o Docker:
```bash
sudo apt install -y docker.io
```

### Agora copia e cola estes comandos, um por vez:
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
#### Após instalado, acesse o navegador com seu ip e porta 1234

   Ex.: http://186.200.120.44:1234

## SUPORTE E SCRIPTS 📎
Precisa de Scripts? Temos dos streaming:

Globoplay

SKY+

PlayPlus(Record)

Youtube

☎️ Contato: https://t.me/felipeadmin
