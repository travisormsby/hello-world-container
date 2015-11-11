docker-hello-world
==================

[![Deploy to Tutum](https://s.tutum.co/deploy-to-tutum.svg)](https://dashboard.tutum.co/stack/deploy/)

Sample docker image to test docker deployments


Usage
-----

To create the image `noahjs/hello-world-81`, execute the following command on the docker-hello-world folder:

	docker build -t noahjs/hello-world-81 .

You can now push your new image to the registry:

	sudo docker push noahjs/hello-world-81


Running your Hello World docker image
-------------------------------------

Start your image:

	sudo docker run -d -p 80 noahjs/hello-world-81

It will print the new container ID (like `d35bf1374e88`). Get the allocated external port:

	sudo docker port d35bf1374e88 80

It will print the allocated port (like 4751). Test your deployment:

	curl http://localhost:4751/


Hello world!

**by http://www.tutum.co**
