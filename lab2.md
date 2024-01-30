### Part 1 - 

**Image of Code**
![Image](Web capture_29-1-2024_204112_edstem.org.jpeg)
![Image](Web capture_29-1-2024_204130_edstem.org.jpeg)

**Input 1**
![Image](screenshot1.jpeg)
_Methods called_: Given the **path** and **query** ```/add-message?s=Hello&user=me``` makes **Server.java** and **ChatServer.java** call on the methods `handleRequest` and the `main method` in which former checks for the **path** and **query** to attain a message and user. In this instance, that would be `Hello` and `me`. The `main method` starts a server and creates a web server in which the `handleRequest` gets its input. 

_Relevant arguments & relevant fields_: Relevant arguments are the message and user name, which is attained using `url.getPath()` and `url.getQuery()` methods, and it splits the **query** (after the `?`) on the `&` and stores them in the local variables (relevant for returning messages with user name) `parameters`, `message`, and `users` that store each separate parts of the query (one the message and one the user). The last relevant field is the `ArrayList messages` that stores a list of Strings, each with the format of `"Name: Message" `and returns a `String result` (formatting `messages` to the proper type & **concatenating**) to display on the web server.

_Relevant fields changed with the request_: Within the `handleRequest` method, there are _if-statements_ that have local variables `parameters`, `message`, and `users` which change given input in the URL on the web server which is in this request ```/add-message?s=Hello&user=me```. Each time the web server has a request, the `ArrayList messages` also changes, updating its array by adding a new String containing a concatenation of the name and message. This inevitably affects the `result` variable as well. `ArrayList messages` contains strings of `me: Hello`, `me: Hello`, `me: Hello`, `you: Hello`, and the newly added string `me: Hello` from the request. The screenshots show the strings displayed in the webserver.

**Input 2**
![Image](screenshot2.jpeg)
_Methods called_: Similar to the first input, the methods that are called on by the user input of `/add-message?s=This%20is%20a%20message&user=cat` are handleRequest and main method in which they check the input for its query and path to attain the message and user. This case would be a message of This is a message and a user of cat. The main method starts a server and creates the web server in which handleRequest gets its input.

_Relevant arguments & relevant fields_: Similarly, relevant arguments are the user's input in the query and path of the web server (`/add-message?s=This%20is%20a%20message&user=cat`), which gives the code its argument to get a message and user using `url.getPath()` and `url.getQuery()` methods. Following this, using local variables of `parameters`, `message`, and `users` to find the message and user, in this case `This is a message` and `cat`, to store them and concatenate them as a string in the instance variable `ArrayList messages`. Following that, it then concatenates all the strings in `messages` in `String result` and returns `result` to display on the web server.

_Relevant fields changed with the request_: The _if-statements_ within the method `handleRequest` have local variables `parameters`, `message`, and `users` that change with each request and stores parts of the **query** to get the message and user from the input in the URL on the web server which is a field that is changed and in this instance is `/add-message?s=This%20is%20a%20message&user=cat`. Each time there is a request, `ArrayList messages` updates with the newly added concatenation of the string in the format `Name: Message` from the input. This affects `result` where the returned variable is a longer string. In this request, the `ArrayList message` contains `me: Hello`, `me: Hello`, `me: Hello`, `you: Hello`, `me: Hello`, and the new addition `cat: This+is+a+message` from the request. The screenshot displays `result`. 

### Part 2 - 
```ls command```
![Image](Web capture_29-1-2024_212725_edstem.org.jpeg)

The first `command` shows the argument and command of `ls /home/.ssh/id_ed25519.pub` which contains the argument _public key_ for logging into `ieng6`.
The second `command` shows the argument and command of `ls /home/.ssh/id_ed25519` which contains the argument _private key_ for logging into `ieng6`.

logging in ```ieng6``` without password
![Image](Web capture_29-1-2024_211425_edstem.org.jpeg)

### Part 3 - 
Something that I didn't know before labs 2 and 3 was connecting to servers and that we can use **URLs** and **URIs** to encode and create a web server that can change based on the **Path** and **Query** input of the web server's URL. 
This ties in with the notion of _ports_ as well where I wasn't aware computers needed ports or how that connected with the notion of webservers. This came with new knowledge about commands like ```ssh``` ```scp``` ```mkdir```
and more. These are very useful for setting up remote servers and setting up ```ssh keys```.
