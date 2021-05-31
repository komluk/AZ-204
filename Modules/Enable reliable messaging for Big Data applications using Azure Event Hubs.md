# Check your knowledge

1. Applications that publish messages to Azure Event Hub very frequently will get the best performance using Advanced Message Queuing Protocol (AMQP) because it establishes a persistent socket.
    - [x] True
    - [ ] False

Answer: Publishers can use either HTTPS or AMQP. AMQP opens a socket and can send multiple messages over that socket.

2. By default, how many partitions will a new Event Hub have?
    - [ ] 1
    - [ ] 2
    - [ ] 3
    - [x] 4

Answer: Event Hubs default to 4 partitions. Partitions are the buckets within an Event Hub. Each publication will go into only one partition. Each consumer group may read from one or more than one partition.

3. What is the maximum size for a single publication (individual or batch) that is allowed by Azure Event Hub?
    - [ ] 256 KB
    - [ ] 512 KB
    - [x] 1 MB
    - [ ] 2 MB

Answer: The maximum size for a single publication (individual or batch) that is allowed by Azure Event Hub is 1 MB.
