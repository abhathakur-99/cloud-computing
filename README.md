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
# Connect to EC2 Instance (Using PuTTY/SSH)

1. Download the `putty.exe` file and install it on your device.
2. Open PuTTY.
3. Go to **Connection** > **SSH** > **Auth**.
4. Choose the key pair file (`.ppk`) you created while launching the instance.
5. Connect to your EC2 instance using the instance’s public DNS or IP address.

```login as username: ubuntu```
# Install Apache
Check in browser → [http://yourpublicip](http://yourpublicip)

An Apache page will be shown at your public IP.
cd /var/www/html
sudo rm index.html
sudo vi index.html



