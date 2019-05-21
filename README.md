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

