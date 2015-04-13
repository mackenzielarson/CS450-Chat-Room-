# CS450 Chat Room
CS 450 Operating Systems Chat Room Project

#Things to install 
Install node in your directory-- Run the following script:

echo 'export PATH=$HOME/local/bin:$PATH' >> ~/.bashrc
. ~/.bashrc
mkdir ~/local
mkdir ~/node-latest-install
cd ~/node-latest-install
curl http://nodejs.org/dist/node-latest.tar.gz | tar xz --strip-components=1
./configure --prefix=~/local
make install # ok, fine, this step probably takes more than 30 seconds...
curl https://www.npmjs.org/install.sh | sh


Install express: 
Express initializes app to be a function handler that you can supply to an HTTP server 
* $ npm install express

To populated dependencies with what we need: 
* $ npm install --save express@4.10.2

Install socket io: 
Socket.IO is composed of two parts:
* A server that mounts on the Node.JS HTTP Server: socket.io
* A client library that loads on the browser side: socket.io-client

* $ npm install --save socket.io

#To run the app
node index.js
* Go to: 
* http://www.cs.sonoma.edu:8022/

#Features we should add: 
* broadcast message if a user connects or disconnects
* support for nicknames 
* show who is connected 
