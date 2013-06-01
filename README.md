algoio R package
======

### Set up environment

In order to use the functions, you will need to set up your R IDE with these settings.  The authentication token 'authToken' is available from the main dashboard of algorithms.io after you sign in

	> authToken="<your token>"	> algoServer="http://v1.api.algorithms.io/"
	
###algoio.upload.dataframe(dataframe)
This is used to upload R data.frame to algorithms.io as dataset.

	> age=rnorm(100, mean=30, sd=14)	> height=rnorm(10, mean=68, sd=20)	> village=data.frame(age=age,height=height)	> head(village)    	    age    height	1 15.712385  61.90196	2 32.569487 108.82751	3 34.062066  30.34053	4 34.685767  91.42471	5 37.705297  35.19011	6  9.519087  98.07798
Then upload…

	