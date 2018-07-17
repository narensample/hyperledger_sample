# Starter kit - Hyperledger Fabric Sample Project
 A basic end to end sample of Fabric 
 This Sample application doesnt have UI
 It will make connection and interaction with Fabric, which running on docker containers 

## Getting Started
These instructions will get you a copy of the sample project up and running on your local machine for development and testing.
### Prerequisites
Node js through NVM(our fabric-sdk is in nodejs )
docker
docker-compose
### Installation Steps
## Case 1 : Windows:
 ```
 1) Install Nodejs from https://nodejs.org/en/
 2) Install docker from download.docker.com
     https://docs.docker.com/
 3) Install dockercompose from 
     https://docs.docker.com/compose/install/#install-compose
 
 ```
 I would like to recommend  "linux" while dealing with docker

 ## Linux:
 1) Install NVM
  ```
     Download the nvm install script via cURL:
        curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.32.1/install.sh | bash

     Ensure that nvm was installed correctly with nvm --version, which should return the version of nvm installed.
     Install the version of Node.js 8.11.2
     Install the specific version with nvm install v8.11.2
 ```
2) Install docker
 ```
    sudo apt-get update
    
    sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    software-properties-common
    
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
    
    sudo add-apt-repository \
    "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
    $(lsb_release -cs) \
    stable"
   
    sudo apt-get update
   
    sudo apt-get install docker-ce
    Verify that Docker CE is installed correctly by running the hello-world image.
```
    ``` 
    sudo docker run hello-world
    ```
    sudo groupadd docker
    ```
    ```
    sudo usermod -aG docker $USER
    ```
    ```
    docker run hello-world
    ```
 
3) Install docker compose

```
sudo curl -L https://github.com/docker/compose/releases/download/1.21.2/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose
```
```
sudo chmod +x /usr/local/bin/docker-compose
```
```
docker-compose --version
```
Setting Application

git clone https://github.com/narensample/hyperledger_sample.git && cd hyperledger_sample && cd sample


 ```
npm install
 ```
Run below commands on same terminal
  ```
  node enrollAdmin.js
  ```

  ```
  node registerUser.js
  ```
  
   ```
  node invoke.js
  ```
  
   ```
  node query.js
  ```

Thank you!
