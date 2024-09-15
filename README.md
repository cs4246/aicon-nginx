# aicon NGINX Configuration Guide

### 1. Install NGINX

```bash
sudo apt update
sudo apt install nginx
```

### 2. Disable the Default Site

To prevent conflicts, remove the default NGINX site configuration:

```bash
sudo rm /etc/nginx/sites-enabled/default
```

### 3. Add Your Custom Configuration

1. **Copy the configuration file** (replace `cs4246` with your configuration file name):

    ```bash
    sudo cp cs4246 /etc/nginx/sites-available/cs4246
    ```

2. **Create a symbolic link** to enable the site:

    ```bash
    sudo ln -s /etc/nginx/sites-available/cs4246 /etc/nginx/sites-enabled/
    ```

### 4. Reload NGINX to Apply Changes

```bash
sudo systemctl reload nginx
```
