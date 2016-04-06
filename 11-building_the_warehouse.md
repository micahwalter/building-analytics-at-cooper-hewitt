# Building the Warehouse

Data warehousing is not a new concept. The idea of gathering together data-sets into a single place, using a single architecture, is pretty common. However, what is new, is the ability to build a data warehouse completely from scratch, scalable at anytime, using cloud based services, with the push of an administration console button.

For CHSDM, the staff chose to experiment with [Amazon’s Redshift](https://aws.amazon.com/redshift/) as its data warehouse.

"Amazon Redshift a fast, fully managed, petabyte-scale data warehouse that makes it simple and cost-effective to analyze all your data using your existing business intelligence tools."

In practical terms, Redshift is a fork of [Postgresql](http://www.postgresql.org/), a powerful, and common open source relational database system. However, Redshift turns things around a bit by re-designing the underlying architecture of Postgresql so that it acts as a columnar data-store. This means that one can use any Postgresql client (such as [psql](http://postgresguide.com/utilities/psql.html)) to connect to a Redshift server.

Starting up a Redshift cluster takes all of five minutes. One simply needs to log into their AWS console, navigate to the Redshift panel and select from a few options. Like most of the offerings from AWS, once can easily scale their Redshift cluster later if they discover the need more resources. Setting up and connecting to Redshift is the easy part.
