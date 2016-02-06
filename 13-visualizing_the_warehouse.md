# Visualizing the Warehouse

Immediately, one can query Redshift using a simple Postegresql compliant client like psql. psql lets you connect to a Redshift cluster and query the data using standard SQL. The results are sent back in text form. It’s typically the first tool one might use to test a connection and start building basic queries.

However, it’s pretty easy to see that writing SQL on the command line and making sense of results from Redshift can be a little bit of a hassle. Additionally, while it’s pretty easy for a developer or data analyst to log into Redshift via the psql client, it’s pretty much impossible to imagine any other staff member doing the same. The next step in building a data warehouse is to attach some kind of analytics tool on top of it that makes the retrieval of data, generation and sharing of reports much easier.

There are a number of off-the-shelf solutions for working with data in a warehouse like Redshift. CHSDM have taken a close look at many of them.

1. [Periscope](http://periscope.io) is a powerful set of business intelligence tools that can connect to a wide variety of data sources including Redshift. It allows you to build SQL based queries through a web interface and chart results using a series of customizable charts types. The reports can be shared with colleagues and easily updated to reflect live data.
2. [Chart.io](http://chart.io) is very similar to Persicope. 
3. [Mode.com](http://modeanalytics.com) is also very similar to Periscope and Chart.io but a little more simplistic and much less expensive. After a trial period CHSDM found Mode to do most of what they wanted to accomplish. The main feature CHSDM were interested in, being able to design an SQL statement and then export the results to Excel, seemed to work perfectly out of the box.

Below is a series of diagrams illustrating some of the reports CHSDM have generated using Mode, connected to its RedShift cluster on AWS. These are mainly first efforts and prototypes, but they illustrate the scenario CHSDM is trying to achieve.

