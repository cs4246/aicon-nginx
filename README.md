# aiVLE NGINX Configuration

Install NGINX
```
sudo apt install nginx
```

Clone the repository
```
git clone https://github.com/cs4246/aivle-nginx.git
```

Copy the configuration to the 
```
cd aivle-nginx
sudo cp cs4246 /etc/nginx/sites-available/cs4246
sudo ln -s /etc/nginx/sites-available/cs4246 /etc/nginx/sites-enabled/
```

Reload NGINX
```
sudo service nginx reload
```