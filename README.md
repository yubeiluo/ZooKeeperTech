ZooKeeperTech
=============
Everything about ZooKeeper

Presentations
=============
1. [ZooKeeper demo code for TriHUG May 22, 2012](https://github.com/mumrah/trihug-zookeeper-demo)
2. [Introduction to ZooKeeper - TriHUG May 22, 2012](http://www.slideshare.net/mumrah/introduction-to-zookeeper-trihug-may-22-2012)
 
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
