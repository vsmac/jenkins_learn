# jenkins_learn

# "installation of jenkins" 

# install of java 

sudo apt update
sudo apt install fontconfig openjdk-21-jre

# TO check java version

java -version

# import key

sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key


echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null

# Install jenkins

sudo apt-get update
sudo apt-get install jenkins

# To check status of jenkins

sudo  systemctl status jenkins.service