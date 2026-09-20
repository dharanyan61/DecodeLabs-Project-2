# The Server Commander

## Description

This project is a cloud computing project completed as part of DecodeLabs Industrial Training.

The objective of this project is to provision a virtual server in the cloud and host a custom web page on it.

In this project, I:

* Launched a Linux Virtual Machine (EC2).
* Connected to the server securely using SSH.
* Installed a web server using the command line.
* Hosted a custom "Welcome to DecodeLabs" webpage.
* Accessed the webpage through the server's public IP address.

## How to Run

### 1. Launch the Linux Virtual Machine

Create and launch an Ubuntu/Amazon Linux EC2 instance in AWS.

### 2. Connect using SSH

Connect to the server using SSH from the terminal.

Example:

```bash
ssh -i your-key.pem ubuntu@YOUR_PUBLIC_IP
```

### 3. Install Apache

Update the packages:

```bash
sudo apt update
```

Install Apache:

```bash
sudo apt install apache2 -y
```

### 4. Start Apache

```bash
sudo systemctl start apache2
```

Enable Apache:

```bash
sudo systemctl enable apache2
```

### 5. Create the Web Page

Edit the default webpage:

```bash
sudo nano /var/www/html/index.html
```

Add the custom "Welcome to DecodeLabs" webpage.

### 6. Access the Website

Open a web browser and enter:

```text
http://YOUR_PUBLIC_IP
```

The hosted webpage should be displayed.

## Tools Used

* AWS EC2
* Linux / Ubuntu
* SSH
* Apache Web Server
* Terminal
* HTML
