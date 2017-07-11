# GRAPHQL USER
 A simple graphql server for the sole purpose of learning graphql

 ### Technologies
 1. GraphQL
 2. Nodejs 8
 3. json-server
 4. Express / Express-graphql


 #### **How to use**
 - clone repository
 - create a db.json file from the sample file
 - run npm install
 - run npm json:server to start the json server
 - run npm start to start the graphQL server
 - navigate to [localhost](http://localhost:4000/graphql)
 
### **Graphql Methods:**
1. **Mutations:**
    - addUser
    - editUser
    - deleteUser
2. **User Fields:**
    - firtsName
    - age
    - companyId
3. **Company Fields:**
    - name
    - description

### **Examples**
1. **Mutations**
    ```
    mutation{
    	editUser(id: "15", firstName: "Nkem") {
            firstName,
            age
        },
        
        addUser(agge: 33, firstName: "Jonh") {
            firstName,
            age
        }
    }
    ```
    
2. **Get**
    ```
    {
	    user(id: "15") {
	        id
            firstName,
            age
        }
    }