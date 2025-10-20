Step 1: Launch your server

You can deploy on any supported platform (AWS EC2 instance)

ssh -i "yourkey.pem" ec2-user@ip-addresss.us-east-2.compute.amazonaws.com
or ssh ubuntu@<your-server-ip> (If this is your first time connecting, accept the SSH fingerprint prompt)

Step 2: Install NGINX

Once connected to your Linux server

sudo yum update -y
sudo yum install nginx -y
sudo systemctl status nginx
sudo systemctl start nginx
sudo systemctl enable nginx

Step 3: Edit the HTML file

cd /usr/share/nginx/html
sudo nano index.html

Step 4: Restart NGINX (but it's optional)

sudo systemctl restart nginx

Step 5: Test in your browser

http://18.217.179.170/
