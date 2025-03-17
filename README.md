Step 1: Created a Workspace
I started by creating a workspace in Postman to organize my API testing work efficiently. This helped me keep all requests, collections, and environments structured.

Step 2: Created Collections
I created two collections, one for the E-commerce API and another for the University Management System API. Collections help group related API requests, making it easier to manage and test them systematically.

Step 3: Configured Environment Variables
To make my API requests dynamic, I set up environment variables for both projects. This included storing base URLs ({{base_url}}), authentication tokens ({{auth_token}}), and other reusable values like product IDs or student IDs.

Step 4: Tested Authentication APIs
I first tested login and authentication endpoints using POST requests to verify user credentials. The API returned a Bearer Token, which I stored in environment variables for authorization in future requests.

Step 5: Tested GET Requests
For the E-commerce API, I fetched a list of products using the GET request (/products).
For the University API, I retrieved student details using the GET request (/students).
I validated the response status codes (200 OK) and checked if the response data matched the expected output.

Step 6: Tested POST Requests
For the E-commerce API, I used a POST request (/products) to add new products with JSON payloads.
For the University API, I used a POST request (/students) to register new students.
I verified the response codes (201 Created) and checked if the database correctly stored new entries.

Step 7: Tested PUT and PATCH Requests
For the E-commerce API, I updated product details using a PUT request (/products/{id}).
For the University API, I modified student records using a PATCH request (/students/{id}).
I checked if the changes were correctly reflected in the database by performing a GET request again.

Step 8: Tested DELETE Requests
I tested DELETE requests to remove specific records:

For the E-commerce API, I deleted a product (/products/{id}).
For the University API, I deleted a student record (/students/{id}).
