# krishna-html

This is a simple Hare Krishna website built using html and css

Steps to Serve HTML and CSS Files on a CentOS Stream 10 Server

1. Download Files to the Server : 

SSH into your CentOS Stream 10 server.

2. Navigate to the httpd document root:

cd /var/www/html

3. Download the files from GitHub using curl or wget:

curl -O https://raw.githubusercontent.com/<your-username>/<repo-name>/main/index.html
curl -O https://raw.githubusercontent.com/<your-username>/<repo-name>/main/k.css
or you can also use wget inplace of curl

4. Install and Start the HTTP Server (httpd)

a. Install the httpd package:

sudo dnf install httpd -y

b.Start the httpd service:

sudo systemctl start httpd

c.Stop the Firewall (Optional for Testing)

5. Stop the firewalld service to allow access to port 80:

sudo systemctl stop firewalld

6. Access the Web Page

Open your browser and load the page using the server's IP address:
http://<server-ip>:80

Replace <server-ip> with the actual IP address of your CentOS server.
