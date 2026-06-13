        1  apt update -y
        2  apt upgrade -y
        4  apt install nginx -y
        5  nginx -t
        6  systemctl start nginx
        7  systemctl enable nginx
        8  systemctl status nginx
        9  cd /var/www/html
       10  ls
       11  rm 
       12  rm index.nginx-debian.html
       13  vim index.html
       14  systemctl restart nginx
       15  cd
       16  apt install git -y
       17  git --version
       18  mkdir dev-web-container
       19  cd dev-web-container
       20  git init
       21  cp /var/www/html/index.html .
       22  ls
       23  git add .
       24  git config --global user.name "Dharshika Poopalan"
       25  git config --global user.email "dharshikasms@gmail.com"
       26  git commit -m "Devops app git connection"
       31  git branch
       32  git branch -M main
       33  git branch
       35  git remote remove origin
       41  git remote add origin https://github.com/DharshikaaPushparaj53/github-dockerize.git
       42  git push -u origin main
       43  apt install apt-transport-https ca-certificates curl software-properties-common -y
       46  sudo mkdir -p /etc/apt/keyrings
       48  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
       **49  echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] \https://download.docker.com/linux/ubuntu \$(. /etc/os-release && echo "$VERSION_CODENAME") stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null**
       50  sudo apt update
       51  sudo apt install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
       52  docker --version
       53  sudo docker run hello-world
       54  systemctl start docker
       55  systemctl enable docker
       56  docker --version
       57  vim Dockerfile
       58  ls
       59  docker build -t devops-nginx-app .
       60  docker images
       61  docker run -d -p 8080:80 devops-nginx-app
       62  docker ps
       63  vim system-health-report
       64  ls -l
       65  chmod +x system-health-report
       66  ls -l
       67  ./system-health-report
       68  vim nginxrunning
       69  chmod +x nginxrunning
       70  ./nginxrunning
       71  ls -l
       72  history
