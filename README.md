# Simulating_HDFS
## Features:

 ###  Data Distribution:
 Randomly distributes a list of transactions (data blocks) across multiple simulated DataNodes.
        Each transaction is stored in one randomly chosen node initially.
        The distributed data is displayed for transparency.

 ##  Data Replication:
 Simulates replication of data blocks to ensure redundancy and fault tolerance, mimicking HDFS behavior.
        A replication factor of 2 ensures that every block is copied to at least one additional node.
        A random probability (random.random() < 0.5) determines whether a block is replicated in each iteration.

 ##  Data Retrieval:
 Provides a method to search for a specific transaction across all DataNodes.
        Efficiently returns the node where the transaction resides or indicates if it is not found in the system.

 ##  Output Logging:
  Displays the initial distribution of transactions across DataNodes.
        Logs the state of the system after the replication process.
        Prints clear and user-friendly messages during transaction retrieval.

  ##  Scalable Design:
  Easily extendable to support more DataNodes or a larger number of transactions.
        Randomized logic ensures robustness in different scenarios.
