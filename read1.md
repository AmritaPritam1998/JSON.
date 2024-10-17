The JSON syntax is a subset of the JavaScript syntax.

JSON Syntax Rules
JSON syntax is derived from JavaScript object notation syntax:

Data is in name/value pairs
Data is separated by commas
Curly braces hold objects
Square brackets hold arrays
JSON Data - A Name and a Value
JSON data is written as name/value pairs (aka key/value pairs).

A name/value pair consists of a field name (in double quotes), followed by a colon, followed by a value:

Example
"name":"John"
JSON names require double quotes.

JSON - Evaluates to JavaScript Objects
The JSON format is almost identical to JavaScript objects.

In JSON, keys must be strings, written with double quotes:

JSON
{"name":"John"}
In JavaScript, keys can be strings, numbers, or identifier names:

JavaScript
{name:"John"}

JSON Values
In JSON, values must be one of the following data types:

a string
a number
an object
an array
a boolean
null
In JavaScript values can be all of the above, plus any other valid JavaScript expression, including:

a function
a date
undefined
In JSON, string values must be written with double quotes:

JSON
{"name":"John"}
In JavaScript, you can write string values with double or single quotes:

JavaScript
{name:'John'}
JavaScript Objects
Because JSON syntax is derived from JavaScript object notation, very little extra software is needed to work with JSON within JavaScript.

With JavaScript you can create an object and assign data to it, like this:

Example
person = {name:"John", age:31, city:"New York"};
You can access a JavaScript object like this:

Example
// returns John
person.name;
It can also be accessed like this:

Example
// returns John
person["name"];
Data can be modified like this:

Example
person.name = "Gilbert";
It can also be modified like this:

Example
person["name"] = "Gilbert";
You will learn how to convert JavaScript objects into JSON later in this tutorial.

JavaScript Arrays as JSON
The same way JavaScript objects can be written as JSON, JavaScript arrays can also be written as JSON.

You will learn more about objects and arrays later in this tutorial.

JSON Files
The file type for JSON files is ".json"
The MIME type for JSON text is "application/json"
***************************json vs xml************
Both JSON and XML can be used to receive data from a web server.

The following JSON and XML examples both define an employees object, with an array of 3 employees:

JSON Example
{"employees":[
  { "firstName":"John", "lastName":"Doe" },
  { "firstName":"Anna", "lastName":"Smith" },
  { "firstName":"Peter", "lastName":"Jones" }
]}
XML Example
<employees>
  <employee>
    <firstName>John</firstName> <lastName>Doe</lastName>
  </employee>
  <employee>
    <firstName>Anna</firstName> <lastName>Smith</lastName>
  </employee>
  <employee>
    <firstName>Peter</firstName> <lastName>Jones</lastName>
  </employee>
</employees>
 JSON is Like XML Because
Both JSON and XML are "self describing" (human readable)
Both JSON and XML are hierarchical (values within values)
Both JSON and XML can be parsed and used by lots of programming languages
Both JSON and XML can be fetched with an XMLHttpRequest
JSON is Unlike XML Because
JSON doesn't use end tag
JSON is shorter
JSON is quicker to read and write
JSON can use arrays
The biggest difference is:

 XML has to be parsed with an XML parser. JSON can be parsed by a standard JavaScript function.

Why JSON is Better Than XML
XML is much more difficult to parse than JSON.
JSON is parsed into a ready-to-use JavaScript object.

For AJAX applications, JSON is faster and easier than XML:

Using XML

Fetch an XML document
Use the XML DOM to loop through the document
Extract values and store in variables
Using JSON

Fetch a JSON string
JSON.Parse the JSON string
