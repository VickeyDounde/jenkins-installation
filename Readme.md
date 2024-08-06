## JENKINS
### Add the Jenkins repository key to your system:
```sh
curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee /usr/share/keyrings/jenkins-keyring.asc > /dev/null
```
```sh
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null
```
### Now Update Machine:
```sh
sudo apt-get update
```
### To install Jenkins:
```sh
sudo apt-get install jenkins
```
### Setup Jenkins as a Daemon:
```sh
systemctl cat jenkins
```
### Jenkins Status:
```sh
sudo systemctl status jenkins
```
