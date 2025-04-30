## Question 1

Path: path/to/page
Host: www.example.com
Query: search=javascript
Port: 8080

## Question 2

1. Operation: GET 
2. Operation: POST 
3. Operation: PATCH 
4. Operation: DELETE 
5. Operation: GET 
6. Operation: PUT 
7. Operation: HEAD

## Question 3

const fetchData = async () => {
    const response = await fetch("https://api.example.com/data");
    const data = await response.json();

    console.log(data);
}

## Question 4

1. Get all todo items: https://api.todo.com/items, GET
2. Add a new todo item: https://api.todo.com/items, POST
3. Mark a todo item as complete: https://api.todo.com/items, PATCH
4. Delete a todo item: https://api.todo.com/items, DELETE

## Question 5

A, C, D, B

When the button is clicked, fetchData is called and immediately logs "A" to console. fetchData then pauses to await the return of data from the API.  Meanwhile, the button Eventlistener continues running, logging "C" to console.  Immediately after this, "D" is logged to console.  Finally, "B" is logged to console, only after the data is fetched from the API.
