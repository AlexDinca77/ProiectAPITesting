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


<li><b>POST</b></li>

HTTP method for request: **POST**<br>
Request description: **POST request to the endpoint https://jsonplaceholder.typicode.com/posts allows you to create a new post in the JSONPlaceholder API. The request body should include JSON data with three fields: "title," which represents the title of the post, "body," containing the main content of the post, and "userId," indicating the ID of the user who authored the post. This endpoint is utilized for adding new posts to the system.**<br>
Test types / techniques used: **Blackbox testing**<br>
Response status code: **201 created**<br>

Below you can find a picture of the API request from Postman:<br>

![image](https://github.com/AlexDinca77/api_testing_postman_jsonplaceholder/assets/167679707/101e9762-55b8-494b-bc76-0693356e58f9)
<br>

JavaScript Tests:

![image](https://github.com/AlexDinca77/api_testing_postman_jsonplaceholder/assets/167679707/fd6bb117-d2ff-410c-ae83-4da341601635) <br>



<li><b>PUT</b></li>

HTTP method for request: **PUT**<br>
Request description: **A PUT request to the endpoint https://jsonplaceholder.typicode.com/posts/1 allows you to update an existing post with the ID "1" in the JSONPlaceholder API. The request body should include JSON data with three fields: "title," representing the updated title of the post, "body," containing the updated main content of the post, and "userId," indicating the ID of the user who authored the post (which remains unchanged in this case). This endpoint is utilized for modifying existing posts in the system.**<br>
Test types / techniques used: **Blackbox**<br>
Response status code: **200 OK**<br>

Below you can find a picture of the API request from Postman:<br>

![image](https://github.com/AlexDinca77/api_testing_postman_jsonplaceholder/assets/167679707/89a6dc50-6809-43f9-bb81-3c69666e18d9)
<br>

JavaScript Tests:
![image](https://github.com/AlexDinca77/api_testing_postman_jsonplaceholder/assets/167679707/915d5c62-7a14-41b5-bf5c-2e52640fedea)
<br>

<li><b>DELETE</b></li><br>
Nume Request: **DELETE**<br>
HTTP method for request: DELETE<br>
Request description: A DELETE request to the endpoint https://jsonplaceholder.typicode.com/posts/1 allows you to remove a specific post with the ID "1" from the JSONPlaceholder API. This endpoint is utilized for deleting existing posts from the system.<br>
Test types / techniques used: BlackBox<br>
Response status code:200 OK<br>

Below you can find a picture of the API request from Postman:<br>

![image](https://github.com/AlexDinca77/api_testing_postman_jsonplaceholder/assets/167679707/844d6776-9e06-434e-9998-7ceacc5e8dbd)<br>


JavaScript Tests:<br>

![image](https://github.com/AlexDinca77/api_testing_postman_jsonplaceholder/assets/167679707/b4c39131-3ba1-47f9-b3d8-8ab32eaa8aa8)<br>
<br>
</ol>

<h2>Execution report for the created API collection </h2>

Below you can find the execution report that was generated through the Postman collection runner. <br>
{<br>
	"id": "74929739-9886-4b4d-a7ab-fbef9b77a60e",<br>
	"name": "Proiect final",<br>
	"timestamp": "2024-04-21T09:31:46.178Z",<br>
	"collection_id": "33827757-86597499-448a-4234-b60c-2e57d80f8525",<br>
	"folder_id": 0,<br>
	"environment_id": "0",<br>
	"totalPass": 10,<br>
	"delay": 0,<br>
	"persist": true,<br>
	"status": "finished",<br>
	"startedAt": "2024-04-21T09:31:44.403Z",<br>
	"totalFail": 2,<br>
	"results": [<br>
		{<br>
			"id": "f9c19b7c-e3df-4c4f-aec2-e37711b8a106",<br>
			"name": "GET Request Tests",<br>
			"url": "https://jsonplaceholder.typicode.com/posts/1",<br>
			"time": 98,<br>
			"responseCode": {<br>
				"code": 200,<br>
				"name": "OK"<br>
			},<br>
			"tests": {<br>
				"Status code is 200": true,<br>
				"Response contains the correct post details": true,<br>
				"Response contains the correct post": true,<br>
				"Response should contain 'Titlul meu' as the title": false<br>
			},<br>
			"testPassFailCounts": {<br>
				"Status code is 200": {<br>
					"pass": 1,<br>
					"fail": 0<br>
				},<br>
				"Response contains the correct post details": {<br>
					"pass": 1,<br>
					"fail": 0<br>
				},<br>
				"Response contains the correct post": {<br>
					"pass": 1,<br>
					"fail": 0<br>
				},<br>
				"Response should contain 'Titlul meu' as the title": {<br>
					"pass": 0,<br>
					"fail": 1<br>
				}<br>
			},<br>
			"times": [<br>
				98<br>
			],<br>
			"allTests": [<br>
				{<br>
					"Status code is 200": true,<br>
					"Response contains the correct post details": true,<br>
					"Response contains the correct post": true,<br>
					"Response should contain 'Titlul meu' as the title": false<br>
				}<br>
			]<br>
		},<br>
		{<br>
			"id": "4c087531-2e24-45db-a9a3-e64512f371c1",<br>
			"name": "POST Request Tests",<br>
			"url": "https://jsonplaceholder.typicode.com/posts",<br>
			"time": 399,<br>
			"responseCode": {<br>
				"code": 201,<br>
				"name": "Created"<br>
			},<br>
			"tests": {<br>
				"Status code is 201": true,<br>
				"Response body is not empty": true,<br>
				"Response should contain the correct post details": false<br>
			},<br>
			"testPassFailCounts": {<br>
				"Status code is 201": {<br>
					"pass": 1,<br>
					"fail": 0<br>
				},<br>
				"Response body is not empty": {<br>
					"pass": 1,<br>
					"fail": 0<br>
				},<br>
				"Response should contain the correct post details": {<br>
					"pass": 0,<br>
					"fail": 1<br>
				}<br>
			},<br>
			"times": [<br>
				399<br>
			],<br>
			"allTests": [<br>
				{<br>
					"Status code is 201": true,<br>
					"Response body is not empty": true,<br>
					"Response should contain the correct post details": false<br>
				}<br>
			]<br>
		},<br>
		{<br>
			"id": "a53a19b7-3488-4999-98d2-86b0579793b5",<br>
			"name": "PUT Request Tests",<br>
			"url": "https://jsonplaceholder.typicode.com/posts/1",<br>
			"time": 395,<br>
			"responseCode": {<br>
				"code": 200,<br>
				"name": "OK"<br>
			},<br>
			"tests": {<br>
				"Status code is 200": true,<br>
				"Response body is not empty": true,<br>
				"Response contains the updated post details": true<br>
			},<br>
			"testPassFailCounts": {<br>
				"Status code is 200": {<br>
					"pass": 1,<br>
					"fail": 0<br>
				},<br>
				"Response body is not empty": {<br>
					"pass": 1,<br>
					"fail": 0<br>
				},<br>
				"Response contains the updated post details": {<br>
					"pass": 1,<br>
					"fail": 0<br>
				}<br>
			},<br>
			"times": [<br>
				395<br>
			],<br>
			"allTests": [<br>
				{<br>
					"Status code is 200": true,<br>
					"Response body is not empty": true,<br>
					"Response contains the updated post details": true<br>
				}<br>
			]<br>
		},<br>
		{<br>
			"id": "2c38a2b9-4e0d-40a3-9c4c-05e300831d2f",<br>
			"name": "DELETE Request Tests",<br>
			"url": "https://jsonplaceholder.typicode.com/posts/1",<br>
			"time": 157,<br>
			"responseCode": {<br>
				"code": 200,<br>
				"name": "OK"<br>
			},<br>
			"tests": {<br>
				"Status code is 200": true,<br>
				"Response body is empty object": true<br>
			},<br>
			"testPassFailCounts": {<br>
				"Status code is 200": {<br>
					"pass": 1,<br>
					"fail": 0<br>
				},<br>
				"Response body is empty object": {<br>
					"pass": 1,<br>
					"fail": 0<br>
				}<br>
			},<br>
			"times": [<br>
				157<br>
			],<br>
			"allTests": [<br>
				{<br>
					"Status code is 200": true,<br>
					"Response body is empty object": true<br>
				}<br>
			]<br>
		}<br>
	],<br>
	"count": 1,<br>
	"totalTime": 1049,<br>
	"collection": {<br>
		"requests": [<br>
			{<br>
				"id": "f9c19b7c-e3df-4c4f-aec2-e37711b8a106",<br>
				"method": "GET"<br>
			},<br>
			{<br>
				"id": "4c087531-2e24-45db-a9a3-e64512f371c1",<br>
				"method": "POST"<br>
			},<br>
			{<br>
				"id": "a53a19b7-3488-4999-98d2-86b0579793b5",<br>
				"method": "PUT"<br>
			},<br>
			{<br>
				"id": "2c38a2b9-4e0d-40a3-9c4c-05e300831d2f",<br>
				"method": "DELETE"<br>
			}<br>
		]<br>
	}<br>
}<br>




First bug:<br>

**Title**: Response should contain 'Titlul meu' as the title<br>
**Pre-conditions**:'- Endpoint: https://jsonplaceholder.typicode.com/posts/1<br>
**Execution steps**: 1. Configure the Endpoint with the URL from the pre-conditions<br>
2. Run the request<br>
**Expected results** : Response should contain 'Titlul meu' as the title<br>
**Actual results** : Response contains "sunt aut facere repellat provident occaecati excepturi optio reprehenderit" as the title<br>

Secound bug:<br>
**Title**: Response should contain the correct post details<br>
**Pre-Conditions**:  Endpoint: https://jsonplaceholder.typicode.com/posts<br>
- Body:<br>
{<br>
  "title": "Sample Title",<br>
  "body": "Sample Bodyy",<br>
  "userId": 1<br>
}<br>
**Execution steps**:1. Configure the Endpoint with the URL from the pre-conditions<br>
2. Configure the Body with the Body from the pre-conditions<br>
3. Run the request<br>
**Expected results**: Response body should contain the following key - value pairs:<br>
{<br>
**Actual results**:Response body contains the following key - value pairs:<br>
{<br>
  "title": "Sample Title",<br>
  "body": "Sample Bodyy",<br>
  "userId": 1<br>
}<br>
  
<h2>Conclusions</h2>

**Executed tests:** 12<br>
**Passed:** 10<br>
**Failed:** 2<br>
**The software seems stable. The severity of the bugs is minor. However, the two requests should be correctly updated before the Production release**
