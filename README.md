# Jenkins-Sonarqube-Docker

1.create vm connected with az cli
2.sudo apt update
3.sudo aptjava -version
--> install openjdk-11-jdk -y
4.install jenkins
---># Import Jenkins GPG key
curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null

# Add Jenkins repo to apt sources
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null

5.sudo apt update
sudo apt install jenkins -y
6.sudo systemctl start jenkins
sudo systemctl enable jenkins
sudo systemctl status jenkins
