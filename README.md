tutum-hello-world
==================

Sample docker image to test docker deployments
Created from original tutum repo for Esri Training Services demonstrations.

Usage
-----

To create the image `esritraining/hello-world`, execute the following command on the tutum-hello-world folder:

	docker build -t esritraining/hello-world .


Running your Hello World docker image
-------------------------------------

Start your image:

	sudo docker run -d -p 80 esritraining/hello-world

It will print the new container ID (like `d35bf1374e88`). Get the allocated external port:

	sudo docker port d35bf1374e88 80

It will print the allocated port (like 4751). Test your deployment:

	curl http://localhost:4751/


Hello world!
