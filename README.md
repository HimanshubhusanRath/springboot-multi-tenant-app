# springboot-multi-tenant-app
This application implemnents the schema per tenant approach in a multi-tenant scenario.

# Steps to test this application:

* Execute the DB_Scripts.sql file for each tenant. Create database instance and tables by using this file.
* Run the Main application.
* Use the below Rest end point to create student under each tenant (database)

<code>
POST http://localhost:8082/students/add
</code>

#### Request Headers ####
X-TenantID = tenant_01  ------> Use different tenant id values (tenant_01 / tenant_02) to see the records created in individual tenant schema.
