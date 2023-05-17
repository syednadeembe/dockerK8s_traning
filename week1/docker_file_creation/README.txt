docker build -t my-nginx-image .

docker run -p 80:80 my-nginx-image

You should be able to view the custom HTML page by navigating to http://localhost/ in your web browser.