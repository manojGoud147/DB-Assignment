1.Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.

Answer: Based on the diagram, the relation between the "Product" and "Product_Category" entities is a one-to-many relationship. This means that one product category can have multiple products associated with it, but each product belongs to only one category.
        The relationship is established through the "category_id" attribute in the "Product" entity, Which likely serves as a foreign key referencing the "id" attribute in the "Product_Category" entity. This allows each product to be assigned to a specific category.

2.How could you ensure that each product in the "Product table has a valid category assigned to it?

Answer: To ensure that each product in the "Product" table has a valid category assigned to it, We can use a foreign key constraint. This constarint would enforce referential integrity, ensuring that the value in the "category_id" column of the "Product" table corresponds to a valid value in the "id"
        column of the "Product_Category table. With this constarint in place, Whenever a new product is added to the "Product" table or an existing product is updated, the database system will verify that the value in the "category_id" column exists in the "id" column of the "Product-Category"
        table. If not, it will prevent the operation, ensuring that each product has valid category assigned to it.
