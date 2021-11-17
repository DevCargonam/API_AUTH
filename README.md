# API_AUTH
Microservicio de Authenticacion



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


