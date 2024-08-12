


### Mutation: `createDog(input: NewDog): Dog!`

![image](https://github.com/user-attachments/assets/de618a14-7eb3-4415-a8b9-aae5e81f3356)

### MongoDB Database:

![image](https://github.com/user-attachments/assets/11615bab-ccfe-4dfd-8d8f-9e143aa0e74c)

### Query: `dogs: [Dog!]!`

![image](https://github.com/user-attachments/assets/7a7adc3d-9e70-4e4c-bc9d-0c32820ed9a6)

### Query: `dog(_id: String!): Dog!`

![image](https://github.com/user-attachments/assets/01e75a97-952f-4669-b689-9c967aa730aa)


### Issues that arose:
* make sure you have MongoDB installed on your pc... smh
* make sure your imports are correct
* make sure your data is structured correctly in the schema
* its standard to make an input type for every unique mutation

### Imporant to know:
#### GraphQL Schema:
Defines the structure of the GraphQL API, including types, queries, and mutations. It acts as a contract between the client and the server, specifying what data can be queried or mutated.
#### Resolvers:
Resolvers actually hold the logic for connecting to the database and grabbing the desired data and returning it in the desired state. In this case, I wrote most of the logic in my "Database" package. 
#### Types:
Define the shape of the data. For example, Dog specifies fields like _id, name, and isGoodBoi.
#### Queries: 
Define read operations that clients can perform, such as fetching a Dog by ID or retrieving a list of dogs.
#### Mutations:
Define write operations that clients can perform, such as creating a new Dog.
#### Models:
help map locally created objects to the database (The models in this project are created automatically by gqlgen library)

