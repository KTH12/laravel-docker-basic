#실행
 - docker-compose up -d
 
기본 포트 : 2121

#포트 수정
``` 
./docker-compose.yml

#Nginx Service
  webserver:
    image: nginx:alpine
    container_name: webserver
    restart: unless-stopped
    tty: true
    ports:
      - "2121:80"
      - "443:443"
```

