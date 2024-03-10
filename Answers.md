Question 1
Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.
    Product-This entity represents individual products.
    
    Product_Category-This entity represents categories which are belonging to product table.
    
    Many-to-One Relationship: This means that many products can belong to one category, but each product can belong to only one category. In other words, multiple products can be categorized under a single category,
    but a product cannot belong to multiple categories simultaneously.
    There is many to many relationship between product and Product_Category by using foreign-key we are establishing relationship between them In the Product table there is a foreign key field named category_id. 
    This field serves as a reference to the primary key of the Product_Category table In the Product_Category table, there is a column named id, which presumably serves as the primary key of this table.
    The category_id field in the Product table establishes a link between products and their respective categories. Each product record contains a value in the category_id field that corresponds to the id of the category 
    it belongs to in the Product_Category table.
    By using this foreign key relationship, it becomes possible to associate each product with its respective category. This structure allows for efficient organization and retrieval of data, making it easier to manage
    and query products based on their categories.

Question 2
How could you ensure that each product in the "Product" table has a valid category assigned to it?
    By using Foreign Key Constraint we can achieve this validation.category_id column in the Product table is a foreign key referencing the id column in the Product_Category table This constraint will enforce 
    that every value in the category_id column of the Product table must By enforcing these constraints and validations, you can ensure that each product in the Product table has a valid category assigned to it.
    Any attempt to insert or update a product
    with an invalid category ID will result in a constraint violation error, maintaining data integrity within your database.


