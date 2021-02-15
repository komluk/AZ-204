# What is an event?

Events have the following characteristics:

    * An event is a lightweight notification that indicates that something happened.
    * The event may be sent to multiple receivers, or to none at all.
    * Events are often intended to "fan out," or have a large number of subscribers for each publisher.
    * The publisher of the event has no expectation about the action a receiving component takes.
    * Some events are discrete units and unrelated to other events.
    * Some events are part of a related and ordered series.


# Check your knowledge
1. Suppose you have a distributed application with a web service that authenticates users. When a user logs on, the web service notifies all the client applications so they can display that user's status as "Online". Is the login notification an example of a message or an event?
    - [ ] Message
    - [x] Event

Answer: The login notification is an event: it contains only a simple piece of status data and there is no expectation by the authentication service for the client applications to react to the notice in any particular way.

2. Suppose you have a distributed application with a web service that lets users manage their account. Users can sign up, edit their profile, and delete their account. When a user deletes their account, your web service notifies your data layer so the user's data will be removed from the database. Is the delete-account notification an example of a message or an event?
    - [x] Message
    - [ ] Event

Answer: The delete-account notification is a message. The key factor is that the web service has an expectation about how the data layer will process the message: the data layer must remove the user's data from the database for the system to function correctly. Note that the message itself contains only simple information so this aspect of the communication could be considered an event; however, the fact that the web service requires the data layer to handle the notification in a specific way is sufficient to make this a message.