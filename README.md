# Revise
![image](https://github.com/sk-kavinda-perera/Revise/assets/139713447/de121f05-46dd-4cc3-afbf-5c2d13a13520)


  
#create: This option tells Hibernate to create the database schema from scratch every time the application starts. It drops the existing tables and recreates them based on the entity mappings. Be cautious when using this option in production as it can lead to data loss.
 
#create-drop: Similar to the create option, this will create the database schema when the application starts. However, it will also drop the schema when the application shuts down. It's typically used for testing or development environments where you want to recreate the schema frequently.
 
#validate: With this option, Hibernate will not attempt to create or update the database schema. Instead, it validates that the schema matches the entity mappings. If there are any inconsistencies, Hibernate will throw an exception. This option is useful in production environments where you want to ensure that the schema is already in sync with the entity mappings.
#
#none: This option disables automatic schema generation entirely. Hibernate will not perform any schema management tasks, and it assumes that the database schema is already configured externally. Use this option when you want to manage the schema manually.
#
#Each option has its use case, and you should choose the one that best fits your development or production requirements. Here's a summary:
#
#create: Use for development or when you want to recreate the database schema from scratch on every application start.
#
#create-drop: Suitable for development and testing environments where you want to recreate the schema frequently.
#
#update: Useful during development and for applications where you want Hibernate to automatically update the schema as entity mappings change.
#
#validate: Recommended for production environments where you want to ensure that the schema matches the entity mappings without performing any automatic modifications.
#
#none: Use when you want to manage the schema manually outside of Hibernate.
