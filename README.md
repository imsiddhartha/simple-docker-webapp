<h1> First application using Docker </h1>

<h3>Licensing</h3>
This is licensed under the Apache 2.0 license - see https://www.apache.org/licenses/LICENSE-2.0

<h3>Getting started</h3>
Host a simple web application using node.js inside a container.

<h3>How to run this code.</h3>
This project assumes that you have alraeady installed a stableversion of docker on your machine.


* cd simple-web-app

Builds docker image based on the configuration provided in Docker file.

* RUN docker build .

Port forwarding:  Provide a port number from your local network, all the request on this port on your local network will be forwarded to 8080 in the container.

Image Id will be generated by the build command.
* docker run -p <port_number>:8080 <Image Id>

You can use browser or postman to do a GET request.
* curl http://localhost:<port_number>



** You shall see a message "Hi there, welcome to docker world!!"
