algoio R package
======
### Installation
First install the devtools package:

	> install.packages("devtools")
	> library(devtools)
	
And then run the install_github command to install algoio package

	> install_github("Algoio", "algorithms-io")
	> library(algoio)
		
### Set up environment

In order to use the functions, you will need to set up your R IDE with these settings.  The authentication token 'authToken' is available from the main dashboard of algorithms.io after you sign in

	> authToken <- "<your token>"	> algoServer <- "http://v1.api.algorithms.io/"
	
###algoio.upload.dataframe(dataframe)
This is used to upload R data.frame to algorithms.io as dataset.

	> age <- rnorm(100, mean=30, sd=14)	> height <- rnorm(10, mean=68, sd=20)	> village <- data.frame(age=age,height=height)	> algoio.upload.dataframe(village)
	[1] "Uploaded data frame with returned reference 4001"

###algoio.publish
To upload an R package, do this

	> algoio.publish(<package path>)
	
For instance,

	> algoio.publish("/Users/anthony1/algotest")
	
	[1] "Successfully uploaded package algotest , reference is 157"
	
		
	


	