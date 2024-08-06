## JENKINS
### Add the Jenkins repository key to your system:
```sh
Copy code
curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee /usr/share/keyrings/jenkins-keyring.asc > /dev/null
```
```sh
Copy code
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null
```
###Now Update Machine:
```sh
Copy code
sudo apt-get update
```
###To install Jenkins:
```sh
Copy code
sudo apt-get install jenkins
```
###Setup Jenkins as a Daemon:
```sh
Copy code
systemctl cat jenkins
```
###Jenkins Status:
```sh
Copy code
sudo systemctl status jenkins
```
