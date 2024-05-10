<h1>API Testing Project for api_testing_postman_jsonplaceholder</h1>

The scope of this project is to use all  API knowledge gained throughout the Software Testing course and apply them in practice, using a live application.

Application under test: *JSON Placeholder*

Tools used: Postman

Collection link: *https://jsonplaceholder.typicode.com/posts*

<h2>Tests performed</h2>

<ol>
<li><b>GET First Post</b></li>

HTTP method for request: **GET**<br>
Request description: **This request retrieves the details of a specific post identified by the ID "1" from the JSONPlaceholder API. This request returns a JSON object containing information such as the post's unique identifier, title, body, and the ID of the user who created the post. This endpoint is useful for fetching the details of a particular post for viewing or further processing.**<br>
Test types / techniques used: **Black-box testing**<br>
Response status code: **200 OK**<br>

Below you can find a picture of the API request from Postman:<br>

![image](https://github.com/AlexDinca77/api_testing_postman_jsonplaceholder/assets/167679707/4264434d-e1f4-4c0e-a043-1e5ab210ca7e)
<br>

JavaScript Tests:

![image](https://github.com/AlexDinca77/api_testing_postman_jsonplaceholder/assets/167679707/287f48d3-5cad-48d4-9484-2d8dfd5cda3b)
<br>


<li>**Nume Request 2**</li>

HTTP method for request: **Inserati aici metoda HTTP a requestului**<br>
Request description: **Inserati o scurta descriere a requestului, conform documentatiei de API**<br>
Test types / techniques used: **Inserati tipurile si tehnicile de testare folosite pentru acest request**<br>
Response status code: **Inserati aici status code-ul pe care l-ati obtinut in urma executiei requestului**<br>

Below you can find a picture of the API request from Postman:<br>

**Inserati aici o poza cu requestul din postman in care sa se observe request method, endpoint, request body si response body**<br>

JavaScript Tests:

**Inserati aici o poza cu testele in java script pe care le-ati definit impreuna cu rezultatele executiei acestora**<br>

.............

<li>**Nume Request n**</li>

HTTP method for request: **Inserati aici metoda HTTP a requestului**<br>
Request description: **Inserati o scurta descriere a requestului, conform documentatiei de API**<br>
Test types / techniques used: **Inserati tipurile si tehnicile de testare folosite pentru acest request**<br>
Response status code: **Inserati aici status code-ul pe care l-ati obtinut in urma executiei requestului**<br>

Below you can find a picture of the API request from Postman:<br>

**Inserati aici o poza cu requestul din postman in care sa se observe request method, endpoint, request body si response body**<br>

JavaScript Tests:

**Inserati aici o poza cu testele in java script pe care le-ati definit impreuna cu rezultatele executiei acestora**<br>

</ol>

<h2>Execution report for the created API collection </h2>

Below you can find the execution report that was generated through the Postman collection runner. <br>

{
	"id": "74929739-9886-4b4d-a7ab-fbef9b77a60e",
	"name": "Proiect final",
	"timestamp": "2024-04-21T09:31:46.178Z",
	"collection_id": "33827757-86597499-448a-4234-b60c-2e57d80f8525",
	"folder_id": 0,
	"environment_id": "0",
	"totalPass": 10,
	"delay": 0,
	"persist": true,
	"status": "finished",
	"startedAt": "2024-04-21T09:31:44.403Z",
	"totalFail": 2,
	"results": [
		{
			"id": "f9c19b7c-e3df-4c4f-aec2-e37711b8a106",
			"name": "GET Request Tests",
			"url": "https://jsonplaceholder.typicode.com/posts/1",
			"time": 98,
			"responseCode": {
				"code": 200,
				"name": "OK"
			},
			"tests": {
				"Status code is 200": true,
				"Response contains the correct post details": true,
				"Response contains the correct post": true,
				"Response should contain 'Titlul meu' as the title": false
			},
			"testPassFailCounts": {
				"Status code is 200": {
					"pass": 1,
					"fail": 0
				},
				"Response contains the correct post details": {
					"pass": 1,
					"fail": 0
				},
				"Response contains the correct post": {
					"pass": 1,
					"fail": 0
				},
				"Response should contain 'Titlul meu' as the title": {
					"pass": 0,
					"fail": 1
				}
			},
			"times": [
				98
			],
			"allTests": [
				{
					"Status code is 200": true,
					"Response contains the correct post details": true,
					"Response contains the correct post": true,
					"Response should contain 'Titlul meu' as the title": false
				}
			]
		},
		{
			"id": "4c087531-2e24-45db-a9a3-e64512f371c1",
			"name": "POST Request Tests",
			"url": "https://jsonplaceholder.typicode.com/posts",
			"time": 399,
			"responseCode": {
				"code": 201,
				"name": "Created"
			},
			"tests": {
				"Status code is 201": true,
				"Response body is not empty": true,
				"Response should contain the correct post details": false
			},
			"testPassFailCounts": {
				"Status code is 201": {
					"pass": 1,
					"fail": 0
				},
				"Response body is not empty": {
					"pass": 1,
					"fail": 0
				},
				"Response should contain the correct post details": {
					"pass": 0,
					"fail": 1
				}
			},
			"times": [
				399
			],
			"allTests": [
				{
					"Status code is 201": true,
					"Response body is not empty": true,
					"Response should contain the correct post details": false
				}
			]
		},
		{
			"id": "a53a19b7-3488-4999-98d2-86b0579793b5",
			"name": "PUT Request Tests",
			"url": "https://jsonplaceholder.typicode.com/posts/1",
			"time": 395,
			"responseCode": {
				"code": 200,
				"name": "OK"
			},
			"tests": {
				"Status code is 200": true,
				"Response body is not empty": true,
				"Response contains the updated post details": true
			},
			"testPassFailCounts": {
				"Status code is 200": {
					"pass": 1,
					"fail": 0
				},
				"Response body is not empty": {
					"pass": 1,
					"fail": 0
				},
				"Response contains the updated post details": {
					"pass": 1,
					"fail": 0
				}
			},
			"times": [
				395
			],
			"allTests": [
				{
					"Status code is 200": true,
					"Response body is not empty": true,
					"Response contains the updated post details": true
				}
			]
		},
		{
			"id": "2c38a2b9-4e0d-40a3-9c4c-05e300831d2f",
			"name": "DELETE Request Tests",
			"url": "https://jsonplaceholder.typicode.com/posts/1",
			"time": 157,
			"responseCode": {
				"code": 200,
				"name": "OK"
			},
			"tests": {
				"Status code is 200": true,
				"Response body is empty object": true
			},
			"testPassFailCounts": {
				"Status code is 200": {
					"pass": 1,
					"fail": 0
				},
				"Response body is empty object": {
					"pass": 1,
					"fail": 0
				}
			},
			"times": [
				157
			],
			"allTests": [
				{
					"Status code is 200": true,
					"Response body is empty object": true
				}
			]
		}
	],
	"count": 1,
	"totalTime": 1049,
	"collection": {
		"requests": [
			{
				"id": "f9c19b7c-e3df-4c4f-aec2-e37711b8a106",
				"method": "GET"
			},
			{
				"id": "4c087531-2e24-45db-a9a3-e64512f371c1",
				"method": "POST"
			},
			{
				"id": "a53a19b7-3488-4999-98d2-86b0579793b5",
				"method": "PUT"
			},
			{
				"id": "2c38a2b9-4e0d-40a3-9c4c-05e300831d2f",
				"method": "DELETE"
			}
		]
	}
}<br>

<h2>Defects found</h2>

The following issues were identified while running the postman tests:<br>

****Inserati aici fie un fisier pdf care sa contina raportarea tuturor bug-urilor, fie le descrieti direct in git
Bug-urile trebuie sa contina titlu, preconditii, pasi de executie, rezultate asteptate si rezultate actuale.
Optional, bug-urile pot fi raportate in jira, si apoi puteti pune poze direct din jira**

<h2>Conclusions</h2>

**Executed tests:** 12<br>
**Passed:** 10<br>
**Failed:** 2<br>
**The software seems stable. The severity of the bugs is minor. However, the two requests should be correctly updated before the Production release**
