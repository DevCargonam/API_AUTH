# API_AUTH
Microservicio de Authenticacion


## Mutation 
```js
mutation { # ##create new user
  userAdd(data:{'UserAddInput'}) {
    idUser
    email
    lastNames
    firstNames
    sex
    birthdate
    DNI
    bloodType
    cellPhone
    homePhone
    emergencyPhone
    idCountry
    idState
    idCity
    address1
    address2
    zipcode

  
  }
}
```
## - Query 
```js
query { # get users
  getUsers(skip: 0, limit: 5) {
    id
    name
  }
}
```

## Scheme
###### tipo de Dato UserAddInput de Entrada para Agregar un Usuario
```js

UserAddInput {
   email:String
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
    address1
    address2
    zipcode
    phone
    redSocial
    observations

}
```
###### tipo de Dato Addrees 
```js
 Addrees {
    adreess1: String 
    adreess2: String 
    adreess3: String 
    adreess4: String 
    city: String 
    locality:String
    country:String 
    zipcode: String
    addressReference:String  
    OtherDetails:String
  }
```
