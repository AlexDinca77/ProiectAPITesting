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

 <br>![image](https://github.com/AlexDinca77/api_testing_postman_jsonplaceholder/assets/167679707/e3e7e1ac-4e70-431b-a8ea-97c34dcc66d9)<br>
<br>![image](https://github.com/AlexDinca77/api_testing_postman_jsonplaceholder/assets/167679707/e255a86e-44d7-4ee5-a19d-9103f04e4889)<br>
<br>![image](https://github.com/AlexDinca77/api_testing_postman_jsonplaceholder/assets/167679707/d35358a3-29c4-4ef2-a0fc-9e381470d3ae)<br>
<br>![image](https://github.com/AlexDinca77/api_testing_postman_jsonplaceholder/assets/167679707/d980a47b-9a84-4d17-8abb-e5a4c696fa88)<br>




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
