# nodejs-tcpgroupchat1
## Nodejs tcp server and client example

This is a simple tcp server and client implementation using nodejs API. This just uses basic nodejs 'net' API.

#Prerequites for running server and client
You just need to install nodejs on your machine.

## Starting Server

Run the following command on the terminal

```
$node groupChatServer.js
```

Server will start running and you should see the following print on the terminal.

```
Server listening on 127.0.0.1:8765
```


Server will bydefault listen on 127.0.0.1, a loopback interface. If you want to change to any other address(you should be to accept connections from other hosts) change SERVER_HOST in the groupChatServer.js to which ever the address you want, also the port number 8765 to something else if you want.

## Starting Client
Now the server is listening for user connections, start client on the other terminal.

start the client as follows.

```
$node groupChatClient.js [your name]
```
'your name' will be sent as sender for all your messages. If you omit 'your name', user name will be 'unknown'.

Now you should see the following prompt.

```
me>
```
And you can type your message here and it will be broadcast to the all users who have connected to the server using the client.
