## Cassandra Tutorial ###
* Introduction
	* Why the tradtional database fails:
		* Data replication
		* SCaling of srd norm form
		* Sharding problem
		* ACID is naive but doesnt do the job
	* Cassndra does:
		* Linear. high availablity
		* No master or slave concept 

* Tech 101:
	* Replication:
		* How many copies of data do you need to keep in cassandra
		* created along with keyspace
		* A keyspace is the collections of tables
	* Consistency Level:
		* CL = ONE
			* means a client is ok if it gets acknowledged only from one node
		* CL =QUORUM
			* maximum acks from the nodes
	* CAP - consistency vs Availabilty 
	* write and read path is so fast 

### Cassandra CQL commnds ##

## Keyspace ##
 * 