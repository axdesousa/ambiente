# ambiente
Ambiente de desenvolvimento com docker-compose

Instalando o docker no ubuntu 18.04 <br><br>
$ sudo apt update <br>
$ sudo apt install apt-transport-https ca-certificates curl software-properties-common <br>
$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - <br>
$ sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"  <br>
$ sudo apt update <br>
$ apt-cache policy docker-ce <br>
$ sudo apt install docker-ce <br>

Adicionado o usuario ao docker, para que não precise usar os comando docker com sudo <br><br>
$ sudo usermod -aG docker ${USER} <br>
$ su - ${USER} <br>
$ id -nG <br>
$ sudo usermod -aG docker nome-do-usuário <br>

Instalando o docker-compose <br><br>
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.23.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose <br>
$ sudo chmod +x /usr/local/bin/docker-compose <br>
