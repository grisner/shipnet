I read about a network of tablets where each tablet contributed to the collected CPU cycles of the net, and subsequently used what was needed from the net. This made the net of tablets as a whole faster, as not all connected tablets was used at the same time.

My idea is a daemon which does:

As a worker node
* publish it's existence on the local network (or maybe connects to some tracker)
* connects to blockchain network
* collect next task
* possibly collects data from bittorrent network
* runs lambda function in task
* publishes result data on either blockchain or bt-network

As a customer node
* publish it's existence on the local network (or maybe connects to some tracker)
* connects to blockchain network
* publish a lambda function to the blockchain
* publish the data either to the blockchain or as a torrent

The plan is to build a framework for (firstly) .Net.

So what I need is 
* an RPC client
* a blockchain
* some way of publishing the node to the network
* 