what is jenkins?
Jenkins is an open-source automation server that enables developers to build, test, and deploy their software

# how to install java

# is used in Debian-based Linux distributions (like Ubuntu) to update the package index. 
sudo apt update

# is used to install specific packages on a Debian-based Linux system (like Ubuntu).
sudo apt install fontconfig openjdk-21-jre

#  is used to check the version of the Java
java -version

# how to install jenkins

# is used in Debian-based Linux distributions (like Ubuntu) to update the package index. 
sudo apt update

# is used to download a GPG key for Jenkins and save it to a specified location.
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key

# is used to add the Jenkins repository to your system's package sources list.
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null

# is used in Debian-based Linux distributions (such as Ubuntu) to update the local package index.
sudo apt-get update
git
# is used to install the Jenkins 
sudo apt-get install jenkins

# You can enable the Jenkins service to start at boot with the command 
sudo systemctl enable jenkins

# You can start the Jenkins service with the command:
sudo systemctl start jenkins

# You can check the status of the Jenkins service using the command:
sudo systemctl status jenkins

