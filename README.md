# PetStore
<h1>Pre-requisites</h1>

You can run the collections by importing it to the postman tool already installed or launch postman on your browser to run these tests.<br>
To run the tests, you need to select the PetStore collection on the left pane and click Run on the right-hand side top corner. You can either choose what modules to run or choose all to run all of them. The summary of test reports can be viewed.<br>
Below is the explanation of the modules in this collection

<h1>PetStore Collection</h1>

PetStore is a collection of regression tests for Pet endpoints from PetStore Swagger - https://petstore.swagger.io/#
<br>The regression covers the happy path, error validations and data validations.
This framework has been designed to cover all the important endpoints in CRUD operations. The top-down approach is used to have a good coverage of all the test scenarios. Similar tests are grouped together to maintain the readability. The environmental and collections variables are used so that any changes in future would be easy to encorporate.<br>
The collection has api_key authorisation where the key is kept secret and is passed as environmental variable.

<h2>AddPet Module</h2>

The AddPet Endpoints is to create data and validate the data created.<br>
Test cases covered are:<br>
•	create data with all the fields<br>
•	null data<br>
•	id with special characters<br>
•	bad request body<br>

<h2>UploadImage Module</h2>

UploadImage is the endpoint where an image can be uploaded as form-data.<br>
The test cases covered are:<br>
•	Uploading image<br>
•	null values to metadata and file<br>
•	no file path given<br>
•	no metadata given<br>

<h2>RetrievePet Module</h2>

RetrievePet endpoints is for retrieving data<br>
Test cases covered are:<br>
•	Retrieving Pet by id<br>
•	The error when pet is not found<br>
Other test cases covered are<br>
•	retrieving or filtering pets by status<br>

<h2>UpdatePet Module</h2>

UpdatePet endpoints is to update the data.<br>
Test cases covered are:<br>
•	find Pet by id and update the data (name and status)<br>
Also covered the test cases where the updated data is passed in request body and some negative scenarios like<br>
•	status data validation<br>
•	name data validation<br>
•	and passing an invalid id<br>

<h2>DeletePet Module</h2>

DeletePet endpoints delete the data. Also covered the testcases for Pet not found and invalid id passed.

