# DM-DBScan

We	start	working	with	more	sophisticated	algorithm,	called	DBSCAN,	which	can	
somewhat	handle	problems	of kmeans.	Since	DBSCAN	is	a	little	complicated	we	don’t	
implement	the	algorithm	in	this	part,	and	we	use	available	libraries.

![sample-result](https://github.com/HosseinMohammadii/DM-DBScan/blob/master/sample-result.png)


In	this	assignment,	we've	been	supplied	with	geographical	distribution	of	COVID-19	patients	
inside	Iran	(covid.csv).	each	row	in	the	csv	file	represents	a	detected	COVID-19	case,	first	
column	is	the	geographical	latitude	and	second	column	is	the	geographical	longitude.	
for	better	visualization	of	geographical	data	we're	using	a	python	library	called	"folium".	

DBSCAN	requires	2	main	parameters,	eps	and	minPts.	
eps	is	the	maximum	allowed	distance	between	2	data	points	in	the	same	cluster,	and	minPts	is	
the	minimum	number	of	data	points	to	create	a	cluster.	Using	these	two	important	parameters	
DBSCAN	dynamically	creates	as	many	as	needed	clusters	while	discarding	any	clusters	without	
enough	data	points	and	keeping	the	outliner	data	points	out	of	any	valid	cluster.	As	a	result,	
changing	the	value	of	these	to	parameters	changes	the	final	number	of	clusters	and	the	way	the	
algorithm	works.	
Our	purpose	is	to	use	DBSCAN	to	find	dense	disease	clusters	inside	Iran.	


# Actual outputs
For see real outputs on map run on your sysmtem connected to internet.
Below images are output for 2 csv files with base parameters in the code.

First:
![first-result](https://github.com/HosseinMohammadii/DM-DBScan/blob/master/Screenshot-2020-05-04-14-01-51.png)

Scecond: 
![second-result](https://github.com/HosseinMohammadii/DM-DBScan/blob/master/Screenshot-2020-05-04-14-00-58.png)
