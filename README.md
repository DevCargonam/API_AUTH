# API_AUTH
Microservicio de Authenticacion


## Mutation 
```js
mutation { # create new user
  userAdd(data:{UserAddInput}) {
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
## Query 
```js
query { # get users
  getUsers(skip: 0, limit: 5) {
    id
    name
  }
}
```

## Scheme
```js
UserAddInput {
 email:String
    pwd:String
    firstNames:String
    lastNames:String
    isCompany:Boolean
    CompanyName:String
    legalRepresentative:String
    sex:String
    photo:String
    birthdate:String
    DNI:String
    cedula:String
    socialSecurityCard:String
    bloodType:String
    cellPhone:String ! 
    homePhone:String
    emergencyPhone:String
    idCountry:Int
    idState:Int
    idCity:Int
    address1:String
    address2:String
    zipcode:String
    phone:String
    redSocial:SocialMediaInput
    observations:String

}
```

