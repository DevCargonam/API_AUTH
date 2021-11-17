# API_AUTH
Microservicio de Authenticacion

```
# install dependencies
npm install

# start the server (GraphiQL is started at http://127.0.0.1:3000)
npm start



## Query Examples

```js
mutation { # create new user
  createUser(name: "") {
    id
    name
    errors {
      path
      errors {
      	validator
      	message
      	code
      }
    }
  }
}
```

```js
query { # get users
  getUsers(skip: 0, limit: 5) {
    id
    name
  }
}
```


