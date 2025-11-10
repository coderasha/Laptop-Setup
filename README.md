# Laptop-Setup

### 1. Github
- sudo apt update
- sudo apt install git -y
- sudo dnf install git -y
- git --version
#### To configure github
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

### 2. install vs code

- sudo apt update
- sudo apt install wget gpg -y
- wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
- sudo install -o root -g root -m 644 packages.microsoft.gpg /usr/share/keyrings/
- sudo sh -c 'echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/packages.microsoft.gpg] - -  https://packages.microsoft.com/repos/code stable main" > /etc/apt/sources.list.d/vscode.list'
- sudo apt update
- sudo apt install code -y

### 3. Install Golang
 - sudo rm -rf /usr/local/go
 - curl -LO https://go.dev/dl/$(curl -s https://go.dev/VERSION?m=text).linux-amd64.tar.gz
-sudo tar -C /usr/local -xzf $(curl -s https://go.dev/VERSION?m=text).linux-amd64.tar.gz
-echo 'export PATH=$PATH:/usr/local/go/bin' >> ~/.bashrc
source ~/.bashrc
-go version

### 3. Install VS Code
-sudo apt update
-sudo apt install wget gpg -y
-wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
-sudo install -o root -g root -m 644 packages.microsoft.gpg /usr/share/keyrings/


