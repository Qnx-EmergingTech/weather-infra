version: '3'
services:

 app:
    image: ghcr.io/qnx-emergingtech/weatheringwithu
    ports:
      - "5000:5000"

 nginx:
    image: nginx:latest
    ports:
      - "8080:80"
    volumes:
      - ./nginx.conf:/etc/nginx/nginx.conf
      - ./app:/app
    depends_on:
      - app
