#Install Docker CE with Docker-Cmpose and Docker-App on Linux Mint 19.1

'''
sudo apt-get install     apt-transport-https     ca-certificates     curl     gnupg2     software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo apt-key fingerprint 0EBFCD88
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(. /etc/os-release; echo "$UBUNTU_CODENAME") stable"
sudo apt-get update
sudo apt-get install docker-ce

echo ""
echo "Install Docker-Compose"
sudo curl -L "https://github.com/docker/compose/releases/download/1.23.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose 

echo ""
echo "Install Docker-App"
wget https://github.com/docker/app/releases/download/v0.6.0/docker-app-linux.tar.gz
tar xf docker-app-linux.tar.gz
sudo cp docker-app-linux /usr/local/bin/docker-app
'''
