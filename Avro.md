## Avro schemas

* Avro is used to define the data schema for a record's value. This schema describes the fields allowed in the value, along with their data types


 		{
 		"type": "record",'
		 "namespace": "com.example",
		 "name": "FullName",
 		"fields": [
   		{ "name": "first", "type": "string" },
   		{ "name": "last", "type": "string" }
		 ]}

* fields: 

	* Unions: A union is used to indicate that a field may have more than one type. They are represented as JSON arrays.

For example, suppose you had a field that could be either a string or null. Then the union is represented as:

["string", "null"]
You might use this in the following way:

    {
     "type": "record",
     "namespace": "com.example",
     "name": "FullName",
     "fields": [
       { "name": "first", "type": ["string", "null"] },
       { "name": "last", "type": "string", "default" : "Doe" }
     ]
    } 


- [Ref: Avro schemas](http://docs.oracle.com/cd/E26161_02/html/GettingStartedGuide/avroschemas.html)
