Test Case № 1:
Title: Add a new pet to the store.
Preconditions: The pet's initial data in the database is as follows
id = "{{petId}}",
name = "{{$randomWord}},
status = {{status}} = sold
Steps: 
1. Send a POST request to {{host}}/v2/pet) with a valid pet JSON body.
Expected Result: Response status 200 OK

Negative Test Cases №2:
Title: Verify that an empty request body returns a validation error
Preconditions: API is running
Steps: Send a POST request to ({{host}}/v2/pet) with an empty request body
Expected Result: Response status 400 Bad Request with an error message "Invalid input" or "Missing required fields".

Test Case № 3:
Title: Verify behavior when API endpoint is incorrect (404 Not Found)
Preconditions: API is running
Steps: Send a POST request to an incorrect URL, to {{host}}/v2/pets (extra "s")
Expected Result: Response status 404 Not Found with an error message "Endpoint not found".

Test Case № 4:
Title: Verify that API returns 500 when database connection fails
Preconditions: Simulate a database failure
Steps: 
1. Send a valid POST request to {{host}}/v2/pet.
2. Ensure the backend database is unavailable.
Expected Result: Response status 500 Internal Server Error with an appropriate error message.

Test Case № 4:
Title: Verify that a duplicate pet ID returns a conflict error
Preconditions: A pet with id: 12345 already exists in the system
Steps: 1. Send a POST request with an existing id (12345).
Expected Result: Response status 409 Conflict with a message "Pet with this ID already exists"
