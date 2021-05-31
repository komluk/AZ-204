## Check your knowledge

1. Which of the following queues should you use if you need first-in-first-out order and support for transactions?
    - [x] Azure Service Bus queues
    - [ ] Azure Storage queues

Answer: Azure Service Bus queues handle messages in the same order they're added and also support transactions. This means that if one message in a transaction fails to be added to the queue, all messages in the transaction will not be added.

2. Suppose you're sending a message with Azure Service Bus and you want multiple components to receive it. Which Azure Service Bus exchange feature should you use?
    - [ ] Queue
    - [x] Topic
    - [ ] Relay

Answer: A topic allows multiple destination components to subscribe. This means that each message can be delivered to multiple receivers.

3. True or false: you can add a message to an Azure Service Bus queue that is 2 MB in size.
    - [ ] True
    - [x] False

Answer: An Azure Storage queue message must be smaller than 64 KB. A service bus queue can be up to 256 KB for standard tier, and 1MB for the premium tier.
