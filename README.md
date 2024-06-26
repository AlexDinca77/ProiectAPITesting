<h1>API Testing Project for api_testing_postman_jsonplaceholder</h1>

<h2>Introduction</h2>
JSONPlaceholder is a web application that serves as a simulated back-end service, providing data in JSON format for use in developing and testing web or mobile applications. Created by a frontend developer named Typicode, JSONPlaceholder is useful for programmers to obtain realistic test data without needing their own server or accessing a real service.<br>

The main features of JSONPlaceholder include:<br>
**Consistent test data**: JSONPlaceholder offers a wide range of endpoints that return standardized JSON data. This data often mimics the structures found in real web applications, such as posts, comments, photo albums, and more.<br>
**Simulation of RESTful functionality**: JSONPlaceholder implements standard HTTP operations, such as GET, POST, PUT, DELETE, which are characteristic of RESTful architecture. This allows developers to test their applications to ensure they interact correctly with a RESTful API.<br>
**Accessibility and ease of use**: To access the data, developers can make HTTP requests to the URLs provided by JSONPlaceholder. No authentication or additional configuration is required to start using the service.<br>
**Open Source and free**: JSONPlaceholder is an open-source project, meaning its source code is available for anyone to review, modify, or improve. Additionally, it is free to use and does not require account creation to access the data.<br>

The scope of this project is to use all  API knowledge gained throughout the Software Testing course and apply them in practice, using a live application.<br>

### Cazuri de testare pentru API-ul JSONPlaceholder

#### GET Request Test
- *Scop*: Verificarea obținerii unei postări specifice.<br>
- *URL*: https://jsonplaceholder.typicode.com/posts/1<br>
- *Pași*:<br>
  1. Trimitere cerere GET către URL.<br>
  2. Verificarea codului de status (așteptat: 200 OK).<br>
  3. Verificarea că răspunsul conține detaliile corecte ale postării.<br>
  4. Verificarea titlului postării (așteptat: "Titlul meu").<br>
- *Rezultate așteptate*:<br>
  - Status code: 200.<br>
  - Detaliile postării sunt corecte.<br>
  - Titlul este "Titlul meu".<br>

#### POST Request Test<br>
- *Scop*: Verificarea creării unei postări noi.<br>
- *URL*: https://jsonplaceholder.typicode.com/posts<br>
- *Pași*:<br>
  1. Trimitere cerere POST cu datele postării.<br>
  2. Verificarea codului de status (așteptat: 201 Created).<br>
  3. Verificarea că răspunsul nu este gol.<br>
  4. Verificarea detaliilor corecte ale postării create.<br>
- *Rezultate așteptate*:<br>
  - Status code: 201.<br>
  - Răspunsul nu este gol.<br>
  - Detaliile postării sunt corecte.<br>

#### PUT Request Test<br>
- *Scop*: Verificarea actualizării unei postări existente.<br>
- *URL*: https://jsonplaceholder.typicode.com/posts/1<br>
- *Pași*:<br>
  1. Trimitere cerere PUT cu datele actualizate ale postării.<br>
  2. Verificarea codului de status (așteptat: 200 OK).<br>
  3. Verificarea că răspunsul nu este gol.<br>
  4. Verificarea detaliilor actualizate ale postării.<br>
- *Rezultate așteptate*:<br>
  - Status code: 200.<br>
  - Răspunsul nu este gol.<br>
  - Detaliile postării sunt actualizate corect.<br>

#### DELETE Request Test<br>
- *Scop*: Verificarea ștergerii unei postări existente.<br>
- *URL*: https://jsonplaceholder.typicode.com/posts/1<br>
- *Pași*:
  1. Trimitere cerere DELETE.<br>
  2. Verificarea codului de status (așteptat: 200 OK).<br>
  3. Verificarea că răspunsul este un obiect gol.<br>
- *Rezultate așteptate*:<br>
  - Status code: 200.<br>
  - Răspunsul este un obiect gol.<br>

### Planificarea metodelor de testare<br>

#### Metode de testare<br>
- *Testare manuală*: Testerul urmează pașii descriși pentru fiecare caz de testare și verifică rezultatele manual.<br>
- *Testare automată*: Scrierea scripturilor de testare automatizate folosind un framework precum Postman sau Jest pentru a executa aceiași pași în mod automat.<br>

#### Plan de testare<br>
- *Ziua 1*:<br>
  - Testare manuală a cazurilor de testare GET și POST.<br>
- *Ziua 2*:<br>
  - Testare manuală a cazurilor de testare PUT și DELETE.<br>
  - Scrierea scripturilor de testare automată pentru toate cazurile de testare.<br>
- *Ziua 3*:<br>
  - Executarea testelor automate și analizarea rezultatelor.<br>


Application under test: *JSON Placeholder*

Tools used: Postman<br>

Collection link: *https://jsonplaceholder.typicode.com/posts*<br>

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

<br> ![image](https://github.com/AlexDinca77/api_testing_postman_jsonplaceholder/assets/167679707/9b9951af-6c98-4f91-bec5-1e6c6e65c511)<br>


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
**Execution steps**:<br>
1. Configure the Endpoint with the URL from the pre-conditions<br>
2. Configure the Body with the Body from the pre-conditions<br>
3. Run the request<br>
**Expected results**:Response body should contain the following key - value pairs:<br>
{<br>
  "title": "Sample Title",<br>
  "body": "Sample Body",<br>
  "userId": 1<br>
}<br>
**Actual results**:Response body contains the following key - value pairs:<br>
{<br>
  "title": "Sample Title",<br>
  "body": "Sample Bodyy",<br>
  "userId": 1<br>
}<br>

Third bug:<br>
**Title**: Response should contain the 'numberOfLikes' propertys<br>
**Pre-Conditions**:  Endpoint: https://jsonplaceholder.typicode.com/posts/1<br>
**Execution steps**:<br>
1. Configure the Endpoint with the URL from the pre-conditions<br>
2. Run the request<br>
**Expected results**: Response body should contain the 'numberOfLikes' property.<br>
**Actual results**:Response body contains the following key - value pairs:<br>
{<br>
  "title": "Sample Title",<br>
  "body": "Sample Bodyy",<br>
  "userId": 1<br>
}<br>
  
<h2>Conclusions</h2>

**Executed tests:** 13<br>
**Passed:** 10<br>
**Failed:** 3<br>
**The software seems stable. The severity of the bugs is minor. However, the requests should be correctly updated before the Production release**
