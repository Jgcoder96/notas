**1. Actualización del sistema operativo:**
```
sudo yum update -y
```
**2. Instala Docker:**
```
sudo yum install docker -y
```
**3. Inicia el servicio de Docker:**
```
sudo service docker start
```
**4. Habilita Docker para que inicie si reinicias el servidor:
```
sudo systemctl enable docker
```
**5. Importante: Agrega el usuario ec2-user al grupo de Docker (para no usar sudo siempre):**
```
sudo usermod -aG docker ec2-user
```
**6**
```
newgrp docker
```
7. instalar docker compose
```
sudo curl -L "https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```
**8. Permisos al archivo**
```
sudo chmod +x /usr/local/bin/docker-compose
```
9. version docker compose
```
docker-compose --version
```
10. crear carpeta
```
mkdir <nombre>
```
11. Entra en la carpeta
```
cd <nombre>
```
12. Crea y abre el archivo
```
nano docker-compose.yml
```
