# Foreign Keys

CHSDM now have two separate databases (one having to do with tickets, and one having to do with the Pen) in two separate systems. The only connection between these two systems is the ID of the ticket, and the ID of the Pen. 

The data is stored in completely different physical locations, and with completely different underlying systems (MySQL vs. MSSQL) but the connection between the two is there, and this means CHSDM can theoretically connect the two data-sets together if it wants to.

In databases, this is called a [Foreign Key](https://en.wikipedia.org/wiki/Foreign_key), and it is one of the most common methods for creating relationships among data both inside the same database and between completely separate databases.
