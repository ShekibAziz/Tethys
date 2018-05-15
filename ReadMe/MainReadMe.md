1. ace-builds folder:
	Library for the online editor that is being displaied on the canned queries web page.
2. css folder:
	all styling for the webspages. Bootstrap is being used as the main styling library for the project.
	Some of the html pages contain css styling if you look in the head section of the html page.
3. D3 folder:
	contains sample works that may be usefull if one is not familuar with the D3 library.
	This folder may be deleted and the project will not be affected in anyway.
4. HTML folder:
	advancedqueries.html:
		Open the Tethys project folder in the commandline(cygwin) and type
		in the following and press enter:
			python -m SimpleHTTPServer
			(The line above creates a sample server) we need this to avoid cross origin problem.
		Open a web page. Type in the url section: http://localhost:8000/index.html
		click on the the Queries tab and select advanced Queries. 
		In this section of the web page we have visualization of the schema and Query Refiner section
		which has not been worked on. Query Refiner will help the user make queries and show the output
		of the query. 
		This file mostly contains JS and is using D3 and select2 libraries. to achieve the visualization.
	cannedQueries.html:
		If you have not done so yet from the previous step go ahead and:
		Open the Tethys project folder in the commandline(cygwin) and type
		in the following and press enter:
			python -m SimpleHTTPServer
			(The line above creates a sample server) we need this to avoid cross origin problem.
		Open a web page. Type in the url section: http://localhost:8000/index.html
		click on the the Queries tab and select canned Queries. 
		In this file I have assigned sample quieries to a varibale by chaning which variable is called in
		an AJAX(using Jquery library) call you will get different results. 
		The sample gui with 3 different parametrs also works. The logic could be improved but works.
5.JSONVersionOfSchemas folder: 
	Deployment folder:
		deploymentForWeb.json
			JSON file that should be used for the D3 library visualization.
		deploymentFullVersion.json
			JSON file with all the inculeds(xml schema "includes" contains and accesses differnet files from folder) that are not nesasary for web.
		sampleDeployment.json
			generated json from the folder Parser XSD to JSON
	sample folder:
		sample.json
			sample json file for testing.
6. Parser XSD to JSON folder:
		xsd_to_json_schema_parser.html:
			This file takes xml schema that is assigned to a variable and converts it to a json format. That will later be used for the advanced queries.
		json.json
			sample json file that is used for testing:
		sample.xsd 
			sample xml schema file that is used for testing
7. ReadMe:
	Helpfull material for the the person who is going to take over the project.
8. XMLSchema(XSD) folder:
	All the schemas that are used in the tethys project
9. index.html
	landing page for the website
10. Thank you Marie and Dr.Whitney <3 