# Re-play & Failing Gracefully

Another incredibly useful aspect of logging data has to do with the concept of replay and graceful failure. In a complex system with many moving parts, it’s only a matter of time before something breaks. Typically it’s one small piece of the larger complex system. It would be a shame that one single issue would result in CHSDM visitors not being able to have an enjoyable experience, so systems are designed to do their best to “fail gracefully.” This means that if one small part of the system becomes temporarily unavailable, the rest of the parts can continue to operate. Since each system produces log messages for every action it performs, the part that was temporarily unavailable can usually be “replayed” once it has recovered.

The following example will be used to illustrate this concept.

A visitor arrives at the museum and purchases a ticket. This invokes a series of requests to a collection of different services. First the ticket is created using a Constituent Relationship Management (CRM) system known as Tessitura.  Once the ticket has been purchased and printed, it is scanned, and tested to ensure it is valid. Then the ticket is “paired” with a Pen which is handed to the visitor for the duration of their visit. If during this process there is a failure with the system that pairs the visitor’s ticket with their Pen, a problem would occur that would normally not allow the visitor services staff to issue the Pen. This could potentially cause a backup at the visitor services desk, resulting in many frustrated customers.

Instead of issuing an error, the system simply writes the log message to disk, and allows the system to carry on as if everything has worked. Later, when the Pen pairing API is back online, the system can go through these log messages and “re-play” the events that failed to work, ultimately presenting the visitor with a seamless experience.

However, this scenario doesn’t always work as planned. For example, in this scenario, if the visitor’s Pen was not successfully paired with their ticket and they went to visit their personal website, they wouldn’t see any of the things they’d collected during their visit. The experience they are expecting will eventually become available to them, ideally before they check, at some point in the future.

![Diagram 07](images/diagram-07.png)
Diagram 07

Diagram 07 illustrates what this might mean. In this example once can see that a Pen was used to collect object [18383769](http://collection.cooperhewitt.org/objects/18383769). If the visitor got home and didn’t see this object on their website as expected, they would hopefully send CHSDM an email explaining their issue. Because CHSDM have a log of this event taking place, CHSDM staff are able to press the “Re-Play This Activity” button, which would re-process this event, thus allowing the visitor to see the expected result.

Without this type of intensive logging, CHSDM wouldn’t be able to recreate the experience. In this instance CHSDM have the potential for a visitor to become temporarily frustrated, but have also ensured that it can eventually alleviate this frustration by replaying the events and producing the expected outcome.
