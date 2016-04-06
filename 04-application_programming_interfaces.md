# Application Programming Interfaces

The nexus of all of the systems involved in the experience at CHSDM is its [Application Programming Interfaces](http://labs.cooperhewitt.org/2014/the-api-at-the-center-of-the-museum/) (API). These APIs are the glue that holds the entire system together and allows for each service and system to communicate with one another. Tap the Pen to a table, and the data on the Pen is transmitted through that API to a database. Every time that interaction happens, log messages are created and stored.

An API is a set of procedures within an application that can be accessed from another application. One can think of an API like an old telephone operator. The phone is used to send instructions, the operator receives these instructions, and as long as the instructions sent are readable, the operator carries out the call, connecting the caller to whomever they were trying to reach.

In the case of the Pen, CHSDM has developed several APIs that allow all of the necessary components to communicate, so that when a visitor taps their pen at one of the digital tables, the call gets through to its expected destination, and the visitor is instantly connected with the right data on the other end.

Every time this interaction happens, the API  makes a record of it in a database. Every time a visitor docks their pen at one of the digital tables, there is a log recorded. Each time an object label is tapped with a Pen and the Pen is read by one of the reader boards, another API method is called, more data is stored, and a log recording this event is saved in a database.

CHSDM now has several APIs. There is an API that deals with the purchasing of tickets at the visitor experience desk and online. Once a ticket has been purchased, the visitor experience staff “pairs” your ticket with a Pen. This act is critical, as it makes sure our systems know which Pen the visitor was using. The pairing procedure calls both the ticketing API and the Pen API, and connects these two sets of data together by storing their respective IDs next to each other in both databases.
