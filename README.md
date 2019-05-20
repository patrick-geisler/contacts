# Contacts 

## Features

* Website to create a easy to remember phone number that you can call that will give you access to some important contacts with a password.
* When the user calls in they will be prompted to enter in their 4-6 digit passcode
* From there we will read out the list of contacts with numbers user can enter the number of the contact that should be read off.


## Build 

### Firebase database
* Just a list of contacts with users 


### Node microservice
* Graphql appolo 
* connections to firebase database
* Mutation: create phone number
* Mutation: add contact to list 
* Query: Get contacts of user

```javascript
User {
	id: Float
	contacts: [Contact]
}

Contact {
	id: !Float
	googleId: Float
	name: String
	number: String
}
```

### Frontend
* Use google authentication
* React, Material-UI, Appolo Client hooks & Next.js
* Login and add contacts either from your google contacts list or something manually add them.


### Automated calling service
* Use the either Amazon, google, or twillo to then create a phone number that will call the 