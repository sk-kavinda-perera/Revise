# Revise

# 1 Types of DDL-AUTO Properties
 ![image](https://github.com/sk-kavinda-perera/Revise/assets/139713447/863dd1c2-4a17-4f84-8e59-6a136475bf8d)

 
* create: This option tells Hibernate to create the database schema from scratch every time the application starts. It drops the existing tables and recreates them based on the entity mappings. Be cautious when using this option in production as it can lead to data loss.
 
* create-drop: Similar to the create option, this will create the database schema when the application starts. However, it will also drop the schema when the application shuts down. It's typically used for testing or development environments where you want to recreate the 
  schema frequently.

* validate: With this option, Hibernate will not attempt to create or update the database schema. Instead, it validates that the schema matches the entity mappings. If there are any inconsistencies, Hibernate will throw an exception. This option is useful in production environments where you want to ensure that the schema is already in sync with the entity mappings.

* none: This option disables automatic schema generation entirely. Hibernate will not perform any schema management tasks, and it assumes that the database schema is already configured externally. Use this option when you want to manage the schema manually.
  
* update: Useful during development and for applications where you want Hibernate to automatically update the schema as entity mappings change.





# Questions
1. what is hibernate?
