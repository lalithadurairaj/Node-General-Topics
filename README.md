# Node-General-Topics
Node Basic Information
# Memory Handling in NodeJS
## RSS Architecture 
   ![alt text](https://github.com/lalithadurairaj/RssArchitectureimg/blob/master/rssimage.png)
   
   
   The heap is part of something bigger though: a running Node.js process store all its memory inside a Resident Set. You can think of it as of a big box which contains some more boxes. The Resident Set contains also the actual Javascript code (inside the Code segment) and the Stack, where all the variables live
  ### process is a global Node.js object which contains information about the current Node.js process, and it provides exactly what we were searching for: the memoryUsage() method.

memoryUsage returns an object with various information: rss, heapTotal, heapUsed (and external):

rss stands for Resident Set Size, it is the total memory allocated for the process execution
heapTotal is the total size of the allocated heap
heapUsed is the actual memory used during the execution of our process

# What is Runtime environment
# How nodejs program run in Google Chrome and other browsers using javascript v8 Engine.

So Node.js does not "work on Firefox" (it doesn't work on Google Chrome either): its a server-side technology. Think of it as a replacement for Python/Ruby/Java in that role. So it can/does respond to requests from all sorts of clients (like Google Chrome and Firefox).

What the "built on V8" means is that it uses the same JavaScript interpreter/just-in-time compiler as Google Chrome. But the similarities with chrome pretty much stop there: Node has no rendering engine/css parser/DOM but does have things you need in a server like an HTTP library and a filesystem API.

https://www.freecodecamp.org/news/understanding-the-core-of-nodejs-the-powerful-chrome-v8-engine-79e7eb8af964/

Asynchronus is achieved by callback and Eventloop.


