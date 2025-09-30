# cloud-computing
# 1 launch instance
# Launch EC2 Instance on AWS

1. Go to AWS Console, then EC2, then **Launch Instance**.
2. Choose **Ubuntu** as the operating system.
3. Create and use a **key pair** for SSH access.
4. Use **PuTTY** to connect to the instance.
5. Allow the following inbound ports in the security group:
   - HTTP (80)
   - HTTPS (443)
   - SSH (22)
6. Launch the instance.
<img width="1920" height="889" alt="image" src="https://github.com/user-attachments/assets/06edfb66-e967-461f-9a82-f9088db6bd64" />
# 2. Connect to EC2 Instance (Using PuTTY/SSH)

1. Download the `putty.exe` file and install it on your device.
2. Open PuTTY.
3. Go to **Connection** > **SSH** > **Auth**.
4. Choose the key pair file (`.ppk`) you created while launching the instance.
5. Connect to your EC2 instance using the instance’s public DNS or IP address.

```login as username: ubuntu```
# 3. Install Apache
Check in browser → [http://yourpublicip](http://yourpublicip)

An Apache page will be shown at your public IP.
<br>```cd /var/www/html ```<br>
  ```sudo rm index.html ```<br>
 ``` sudo vi index.html``` <br>
 Press I to insert your own html code.  
 Write your own code.  
 After writing all code, Press Ctrl+C and then write ":wq" and Press Enter.
# 4. Map Domain with Route 53

- Register your own domain name.
- Go to Route 53 on AWS, click on **Hosted Zones**.
<img width="1914" height="874" alt="image" src="https://github.com/user-attachments/assets/a315d447-3ef9-4674-a132-3d9aa4323c29" />
You will get four NS name server.
# Docker Install

## Quick Install

curl -sL https://github.com/ShubhamTatvamasi/docker-install/raw/master/docker-install.sh | bash
install packages: 
<br> ```sudo apt update
sudo apt install -y \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg \
    lsb-release \
    jq```

