ZooKeeperTech
=============
Everything about ZooKeeper

Presentations
=============
1. [ZooKeeper demo code for TriHUG May 22, 2012](https://github.com/mumrah/trihug-zookeeper-demo)
2. [Introduction to ZooKeeper - TriHUG May 22, 2012](http://www.slideshare.net/mumrah/introduction-to-zookeeper-trihug-may-22-2012)
3. [So we're running Apache ZooKeeper. Now What? By Camille Fournier](http://www.slideshare.net/g33ktalk/zoo-keeper-basics-sug)
 
Problems about the group membership demo:

Is it possible that some member will not get the up-to-date member set? For example, let us consider the following action sequences:

1. Member A sets the children watch
2. Member A creates the ephermeral node
3. Member A gets notified of the child event
4. Member B sets the children watch and creates the ephermeral node
5. Member A reset the watch 

Consequently, member A misses the the children event raised by member B and is not aware of B's existence.

Commands
=============
1. echo ruok | nc localhost 2181

Client Frameworks
=============
1.[ZooKeeper client wrapper and rich ZooKeeper framework](https://github.com/Netflix/curator)

Use Cases
============
1. [Managing Configuration of Distributed System with Apache ZooKeeper](http://sysgears.com/articles/managing-configuration-of-distributed-system-with-apache-zookeeper/)
2. [Updating thousands of configuration files in under a second](http://code.zynga.com/2011/08/updating-thousands-of-configuration-files-in-under-a-second/)

