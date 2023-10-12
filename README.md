# Laravel-Project-1
Created API by using Laravel, with the following endpoints:
o GET /companies -> will return the full list of companies
o GET /companies/{id} -> will return the data of the selected company
o POST /companies -> to create a new company
o POST /company/update -> to update the company
o POST /company/delete/{id} -> to delete the selected company
Column Type
id bigint(20) unsigned Auto Increment
name varchar(255)
sector_id int(10) unsigned
website varchar(255) NULL
phone varchar(255)
email varchar(255)
country varchar(255) NULL
city varchar(255) NULL
address varchar(255)
• Sector_id is a foreign key for another table that stores the sectors (Accounting, Arts,
Fashion, ...)
• Sectors table only have ID and name
• The response in JSON format
• The first endpoint (GET /companies) should support filtering the data by the field
value and supports pagination. i.e. /companies?pageSize=10&page=1&name=”abc”
