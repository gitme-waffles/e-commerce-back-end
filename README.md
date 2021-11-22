# E-commerce Back end
 

## Table of Contents
- [Installation Instructions](#installation-instructions)
- [Usage](#usage)
- [Walkthrough Video](#walkthrough-video)
- [Questions](#questions)


## Installation Instructions
### Requires 
- `node.js`
- `MySQL`
- `npm`
  - `express`
  - `mysql2`
  - `sequelize`
  - `dotenv`

After forking and downloding the project, locate the folder and install the dependencies with the following command in the command line:
```
npm i
```
### Connect to the database
After the dependencies have been installed you need to initialise the database with the schema.

Using the same directory path in the command line start MySQL in your preffered CLI with `mysql -u YOUR_USERNAME -p` followed by you password, then use the following command to run the schema:
```
SOURCE db/schema.sql;
```

Back in the command line from the npm install, run the following command to populate the database with provided data:
```
npm run seed
```


## Usage 

### Input MySQL credentials
In the `.env` file insert your SQL credentials for the application to access the database
```sql
DB_USER='USERNAME_HERE'
DB_PW='PASSWORD_HERE'
DB_NAME='ecommerce_db'
```

Run the following command in the next line to start the application:
```
npm start
```

In Insomnia core or your preffered REST client, using this url `localhost:3001/api/` followed by `categories`, `products` or `tags` to get to the desired end point to check that it is getting data from the database. If you want to select a single specific category, product or tag, just add the id of the target at the end of the URL. Examples below:

### GET All Categories, POST a new category
```
localhost:3001/api/categories/
```
### GET Category by ID, PUT/update or DELETE a category
Replace the number at the end with the target id
```
localhost:3001/api/categories/1
```
### GET All Products, POST a new product
```
localhost:3001/api/products/
```
### GET Product by ID, PUT/update or DELETE a product
Replace the number at the end with the target id
```
localhost:3001/api/products/1
```
### GET All Tags, POST a new tag
```
localhost:3001/api/tags/
```
### Get Tag byID, PUT/update or DELETE a tag
Replace the number at the end with the target id
```
localhost:3001/api/tags/1
```
## Walkthrough Video
Link to [walkthrough video](https://watch.screencastify.com/v/H7yNgPbHWjaucx02hzF3)

## Questions
Contact me on [Github](https://github.com/gitme-waffles) if you have any questions  
