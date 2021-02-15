# Check your knowledge

1. Suppose you work for a government agency that plans the long-term expansion of the highway system. You receive traffic data from thousands of sensors and analyze it to make your recommendations. The amount of incoming data varies throughout the day; for example, it spikes during the morning and evening commuting hours. True or false: a server-side architecture consisting of an Azure Queue connected to a single virtual machine is a reasonable choice for this workload?

    [x] True
    [ ] False

Answer: The queue will handle spikes in traffic and ensure no data is lost. If the VM cannot keep up with the flow of incoming messages, it will process the message backlog during low-traffic times.

2. What information uniquely identifies a queue?

    [ ] Queue name
    [ ] Account key
    [x] Storage account name and queue name

Answer: Storage account names must be globally unique. Queue names must be unique within their containing storage account. This means the combination of storage account name and queue name uniquely identifies a queue.

3. True or false: when a client programmatically retrieves a message from a queue, the message is automatically deleted from the queue?

    [ ] True
    [x] False

Answer: By design, messages are not automatically deleted from a queue after they are retrieved for processing. This helps ensure that every message is processed to completion. If a consumer application crashes during processing, the message is still available to be processed by a different instance of the consumer app.
1 out of 3 questions is incorrect.