# aicon NGINX Configuration

Install NGINX
```
sudo apt install nginx
```

Copy the configuration 
```
sudo cp cs4246 /etc/nginx/sites-available/cs4246
sudo ln -s /etc/nginx/sites-available/cs4246 /etc/nginx/sites-enabled/
```

Reload NGINX
```
sudo service nginx reload
```
