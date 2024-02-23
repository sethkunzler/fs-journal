# Intro to Server side concerns with JavaScript
01. What do the letters of the acronym `CRUD` stand for?

  > Create
  > Read
  > Update
  > Delete

02. Each action that `CRUD` represents maps to an HTTP request. What HTTP request does each `CRUD` action correspond to?

  > Create --> post
  > Read --> get
  > Update --> put
  > Delete --> delete

03. What does `ORM` stand for? Which `ORM` do we use when interacting with MongoDB

  > Object Relational Mapping - which is the mapping of how one piece of data relates to another
  > we use Node.js in MongoDB to map the relationship of objects

04. Which two `HTTP` request types include a body?

  > post and put

05. In a/an _______ coding model, when you call a function, it returns only when the action has finished and stops your program for the time the action takes. Likewise in a/an _______ coding model, multiple things are allowed to happen at one time. When you perform an action, your program continues to run.  Fill in the blanks.

  > A.  synchronous
  > B.  asynchronous

06. What are the three types of data relationships? Provide an example of each.

  > one to one : a one to one relationship is where one property will only ever have one specific value which is not attached to any other objet. i.e. 
  ```js
  United States {
    population: 300,000
    // capital is a one to one relationship, each country will only have one capital and each capital will only have one country
    capital: "Washington DC" 
    size: 3,531,000
  }
  ```
  > one to many : a one to many relationship is where one property could have many values
  ```js
  Alaska {
    population: 730,000
    capital: "Juneau"
    size: 586,000
    // country is a one to many relationship, each state/county/city will belong to just one country (most of the time, e/w berlin technically got split into two cities so I still think it applies all the time), but a country can have multiple states/counties/cities 
    country: "The United States"
  }
  ```
  > many to many
  ```js
  Alaska {
    population: 730,000
    capital: "Juneau"
    size: 586,000
    country: "The United States"
    // there might be multiple ways to describe the climate in a specific place, but most descriptions can be applied to other places as well
    // Minnesota might also be cold and wet, where florida might be hot and wet.
    climate: ["cold", "wet"]
  }
  ```

07. What is middleware?

  > a software that makes the transfer of data to and from a database to an app easier to use. 

08. The ______ pipeline delivers information from the client while the ______ pipeline returns it. Fill in the blanks. 

  > A. request
  > B. response

09. Demonstrate the pattern that is used to include a request query with the client's `HTTP` request providing the property `tag` and the value `winter`.

  > 
  ``` js
  "api/${place}?tag=winter"
  ```

10. What is a ***virtual property***?

  > A virtual property is when you target the property/properties of another object that exist inside a different Shcema
