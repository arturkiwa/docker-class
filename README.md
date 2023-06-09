## docker-class

# Instalacja Dockera na Ubuntu

```bash
sudo apt update
```
```bash
sudo apt install apt-transport-https ca-certificates curl software-properties-common
```
```bash
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```
```bash
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
```bash
sudo apt update
```
```bash
apt-cache policy docker-ce
```
```bash
sudo apt install docker-ce
```
```bash
sudo systemctl status docker
```

# Instalacja docker-compose

```bash
mkdir -p ~/.docker/cli-plugins/
```
```bash
curl -SL https://github.com/docker/compose/releases/download/v2.3.3/docker-compose-linux-x86_64 -o ~/.docker/cli-plugins/docker-compose
```
```bash
chmod +x ~/.docker/cli-plugins/docker-compose
```
```bash
docker compose version
```
