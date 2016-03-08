### Maven tips
* core components:
	* basic parent pom.xml
		* start xml tag	
		* model version: Maven model (t is always set to 4.0.0 in Maven 2 and 3, because, at present, there is no other model.)
		* Parent:
			* groupid
			* artifact id
			* version
			* name
			* packaging : like pom, jar, war etc..
		*  properties: something common for child
		*  modules: What are the modules present underneath parent pom file
		*  scm plugin specifics
		*  url
		*  description
		*  build contains:
			*  all maven plugins tree(contains groupid, artifactid)
		* distribution management
	* child pom.xml:
		*   same as above may contains dependencies like for mockito, 
			
 