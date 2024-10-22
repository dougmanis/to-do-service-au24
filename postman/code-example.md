# Code examples

**Author:** Doug Manis

## cURL code examples 

### GET example (cURL)

#### GET request 

The following GET request fetches the details for user of ID 3: 

```shell
curl http://localhost:3000/users/3
```

#### GET response

```shell
{
  "last_name": "Martinez",
  "first_name": "Marty",
  "email": "m.martinez@example.com",
  "id": 3
}
```

### POST example (cURL) 

The following POST request creates a new user named Fred Smithy with email f.smithy@example.com: 

#### POST request 

```shell
curl -d "last_name=Smithy&first_name=Fred&email=f.smithy@example.com" -X POST http://localhost:3000/users
```

#### POST response 

Note that the POST response data includes the user data you submitted in your request and the new user's unique ID (5 in this case). The server generates the unique ID automatically. 

```shell 
{
  "last_name": "Smithy",
  "first_name": "Fred",
  "email": "f.smithy@example.com",
  "id": 5
}
```

## Postman example

The GET example below fetches the details for task of ID 3. Be sure to use the URL for your own system when you try this example. 

### GET request

```shell
{base_url}/tasks/3
```

### GET response

```shell
{
    "user_id": 2,
    "title": "Oil change",
    "description": "5K auto service",
    "due_date": "2024-03-10T09:00",
    "warning": "-60",
    "id": 3
}
```
