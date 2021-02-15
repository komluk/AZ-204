# Benefits of queues
Queue infrastructures can support many advanced features that make them useful in the following ways.

# Use Service Bus topics if you:
    * Need multiple receivers to handle each message

# Use Service Bus queues if you:
    * Need an At-Most-Once delivery guarantee.
    * Need a FIFO guarantee.
    * Need to group messages into transactions.
    * Want to receive messages without polling the queue.
    * Need to provide a role-based access model to the queues.
    * Need to handle messages larger than 64 KB but less than 256 KB.
    * Queue size will not grow larger than 80 GB.
    * Want to publish and consume batches of messages.

# Use Queue storage if you:
    * You need a simple queue with no particular additional requirements
    * You need an audit trail of all messages that pass through the queue
    * You expect the queue to exceed 80 GB in size
    * You want to track progress for processing a message inside of the queue

# Use Event Grid when you need these features:

    * Simplicity: It is straightforward to connect sources to subscribers in Event Grid.
    * Advanced filtering: Subscriptions have close control over the events they receive from a topic.
    * Fan-out: You can subscribe to an unlimited number of endpoints to the same events and topics.
    * Reliability: Event Grid retries event delivery for up to 24 hours for each subscription.
    * Pay-per-event: Pay only for the number of events that you transmit.

# Choose Event Hubs if:
    * You need to support authenticating a large number of publishers.
    * You need to save a stream of events to Data Lake or Blob storage.
    * You need aggregation or analytics on your event stream.
    * You need reliable messaging or resiliency.