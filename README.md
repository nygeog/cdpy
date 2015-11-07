#CdbPy
An un-sanctioned **CartoDB** Python Wrapper for Geoprocessing with **PostGIS** *SQL* created with the intent of helping ease **ArcPy** users into **CartoDB** and **PostGIS** 

##Importing CdbPy Username and API Key
	
	import cdbpy

	username = '<CartoDB Username>'
	apikey   = '<CartoDB API Key>' 

Or use [.gitignore](#gitignore) and save data in **\_secret_info.py**

	import _secret_info
	import cdbpy
	
	username = _secret_info.cartoDBusername
	apikey   = _secret_info.cartoDBapikey

##List Functions:

####Test
`printTest(inText)`
	
####Create Table	
`createTable(table_name,username,apikey)`


![logo](logo/cartodb-arcpy-wrapper-logo.png)


##gitignore<a name="gitignore"></a>
gitignore is a file you store in your repo, name the file **.gitignore**. Yes, with the **.** starting the file extension, with no file name.

	# Secret Python files #
	###################
	*_secret_info.py
	*.pyc
	
	# JSON files #
	###################
	*test.json