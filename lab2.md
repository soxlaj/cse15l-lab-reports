###Part 1 - 

**Image of Code**
![Image](Web capture_29-1-2024_204112_edstem.org.jpeg)
![Image](Web capture_29-1-2024_204130_edstem.org.jpeg)

**Input 1**
![Image](screenshot1.jpeg)
_Methods called_: Given the **path** and **query** ```/add-message?s=Hello&user=me``` makes **Server.java** and **ChatServer.java** call on the methods `handleRequest` and the `main method` in which former checks for the **path** and **query** to attain a message and user. In this instance, that would be `Hello` and `me`. The `main method` starts a server and creates a web server in which the `handleRequest` gets its input. 

_Relevant arguments & relevant fields_: Relevant arguments are the message and user name, which is attained using `url.getPath()` and `url.getQuery()` methods, and it splits the **query** (after the `?`) on the `&` and stores them in the local variables (relevant for returning messages with user name) `parameters`, `message`, and `users` that store each separate parts of the query (one the message and one the user). The last relevant field is the `ArrayList messages` that stores a list of Strings, each with the format of `"Name: Message" `and returns a `String result` (formatting messages to the proper type & **concatenating**) to display on the webserver.

_Relevant fields changed with the request_: Within the `handleRequest` method, there are if-statements that have local variables `parameters`, `message`, and `users` which change given input in the URL on the webserver. Each time the webserver has a request, the `ArrayList messages` also changes, updating its array by adding a new String containing a concatenation of the name and message. This inevitably affects the `result` variable as well. 

**Input 2**
![Image](screenshot2.jpeg)
Methods called:

Relevant arguments & relevant fields:

Relevant fields changed with the request:

###Part 2 - 
```ls command```
![Image](Web capture_29-1-2024_212725_edstem.org.jpeg)

logging in ```ieng6``` without password
![Image](Web capture_29-1-2024_211425_edstem.org.jpeg)

###Part 3 - 
Something that I didn't know before labs 2 and 3 was connecting to servers and that we can use URLs and URIs to encode and create a webserver that can change based on the Path and Query input of the web server's URL. 
This ties in with the notion of ports as well where I wasn't aware computers needed ports or how that connected with the notion of webservers. This came with new knowledge about commands like ```ssh``` ```scp``` ```mkdir```
and more. These are very useful with setting up remote servers and setting up ```ssh keys```.
