# Visualizing the Warehouse

Immediately you can query Redshift using a simple Postegresql compliant client like psql. psql lets you connect to a Redshift cluster and query the data using SQL. The results are sent back in text form, just like they would be if you were to use the standard MySQL client from the command line. It’s typically the first tool one might use to test if you can connect and start building basic queries.

However, it’s pretty easy to see that writing SQL on the command line and getting results from Redshift can be a little bit of a hassle. While it’s pretty easy for a developer or data analyst to log into the psql client, it’s pretty much impossible to imagine any other staff member doing the same. The next step in building our data warehouse is to attach some kind of analytics tool on top of it that makes the retrieval of data, generation and sharing of reports a snap.

There are a number of off the shelf solutions for working with data from a warehouse like Redshift. We’ve taken a close look at many of them.

1. Periscope is a powerful set of business intelligence tools that can connect to a wide variety of data sources including Redshift. It allows you to build SQL based queries through a web interface and chart results using a series of customizable charts types. The reports can be shared with colleagues and easily updated to reflect live data.
2. Chart.io is very similar to Persicope. 

In both cases you simply put in your AWS info, setup the proper security info to allow it to connect to Redshift and you are off and running. Ultimately both of these solutions proved too expensive at the time.

3. Mode.com is also very similar to Periscope and Chart.io but a little more simplistic and much less expensive. After a trial period I found Mode to do most of what we wanted to accomplish. The main feature we were interested in, being able to design an SQL statement and then export the results to Excel, seemed to work perfectly out of the box.

Below are a series of diagrams illustrating some of the reports we’ve generated using Mode, connected to our RedShift cluster on AWS. These are mainly first efforts and prototypes, but they illustrate the scenario we are trying to achieve.
