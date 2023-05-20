docker volume create nginx-data
docker run -d --name nginx -v nginx-data:/data -v $(pwd)/nginx.conf:/etc/nginx/nginx.conf -p 80:80 nginx:latest
docker cp index.html nginx:/data/
docker inspect volume nginx-data
docker inspect container <name>

