# openpiv-saas

## Background:
This application consist of two parts:
1. javascript client.
2. python server.

## Basic flow:
The user sends process command using the web page. This command gets from the javascript client to the server.
The python server to performs the neccessery action and gets back the result, pass it back to the client and shows it on screen.

For this version the flow supported is basic analysis of two images.

## Installation:
1. clone openpiv-saas repository to your server.
2. in .env file in the root of client directory, change the REACT_APP_SERVER_URL to your server url.
3. install docker and docker-compose on your server:
  - example of install docker on ubuntu 16.04 https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-16-04
  -  example of install docker-compose on ubuntu 16.04 https://www.digitalocean.com/community/tutorials/how-to-install-docker-compose-on-ubuntu-16-04
4. in openpiv-saas root directory run command: docker-compose up -d
5. make sure the server can get incomming trafic from ports 80 (for client) and 4000 (for server).
