# Challenge-13-E-commerce-Back-End
## Description

A back end for an e-commerce site to update a database of categories, products and tags.  Products belong to a category, and can belong to any number of tags.  Tags can have any number of products.  
- GET routes for all categories, products and tags.  
  - Ex. GET /api/categories
- GET routes for one category, product and tag using the auto-generated ID.  
  - Ex. GET /api/categories/1  
- POST routes to add a new category, product, or tag.  
  - Ex. POST /api/categories  
- PUT routes to update a category product or tag using the ID.  
  - Ex. PUT /api/categories/1  
- DELETE routes to delete a category, product or tag using the ID,
  - Ex. DELETE/api/categories/1

## Installation
Necessary components will be installed with  
- npm i

## Usage
In the db folder:
- Create a .env file in the root directory with  
    DB_NAME = 'ecommerce_db'  
    DB_USER = your mySQL user name  
    DB_PASSWORD = your mySQL password
- Run schema.sql in mySQL to create the database.
- Run "npm run seeds" to add initial data.
- Run the following command from the terminal to start the server  
    - npm run start  
      
- body JSON for POST and PUT routes as follows:
    - /api/categories:  
    {  
        category_name: "category name"  
    }  
    - /api/products:  
    {  
        product_name: "product_name"  
        price: 200.00,  
        stock: 3,  
        tagIds: [1, 2, 3, 4]  
    }  
    - /api/tags:  
    {  
        tag_name: "tag name"  
    }

## Example
[Example video](https://drive.google.com/file/d/1bCNh1rtN-6NOtlcCt9_wBOq30iM_nS-x/view) showing working routes in Insomnia.