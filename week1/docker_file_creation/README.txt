docker build -t my-nginx-image .

docker run -p 80:80 my-nginx-image
#docker run -p <host_port>:<container_port> <image_name>


You should be able to view the custom HTML page by navigating to http://localhost/ in your web browser.