## 1. set up
``` dockerfile
version: '3'
services:
  app:
    image: 'jc21/nginx-proxy-manager:latest'
    restart: unless-stopped
    ports:
      - '80:80'
      - '81:81'
      - '443:443'
    volumes:
      - ./data:/data
      - ./letsencrypt:/etc/letsencrypt
```
## 2. Proxy Hosts
![avatar](https://raw.githubusercontent.com/chjtxwd/nginx-proxy-manager-and-traefik-demo/main/nginx-proxy-manager/nginx-proxy-manager.png)
## 3. Redirection Hosts
## 4. 404 Hosts
## 5. Access Lists
## 6. Apply for SSL Certificates
