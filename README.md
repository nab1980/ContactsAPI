Contacts API
============

Technology/Components used:
==========================
	1. Asp.Net Web Api
	2. Entity Framework
	3. MSTest Unit Test project to check controller actions
	4. Visal Studio Community Edition
	5. SQL Server inbuilt express edition [(localdb)\MSSQLLocalDB]
	6. Moq framework for unit test project

Patterns/Principle used:
=======================
	1. Repository patterns 
	2. Dependancy Injection with UNity
	3. Code First Approach (Entity Framework)
	4. Created Action Filter for Model Validation
	5. Created Action Filter for global exception handling
	6. Data Annotations for model validation

How to run:
==========
	1. Download project files locally
	2. Open solution with VS 2015 or VS 2017
	3. Build and run project
	4. Url should be http://localhost:50448/
	5. Various end points:
		http://localhost:50448/conact : [GET] get all contacts
		http://localhost:50448/contact/1 : [GET] get contact with specific id
		http://localhost:50448/contact :[POST] pass json object to add new contact
		http://localhost:50448/contact/1 :[PUT] pass updated json object to update existing contact
		http://localhost:50448/contact/1 :[DELETE] to delete contact with specific id
	
	**On first request it may be slow as going to create database schema

Below some improvements which not added but should be good practice to add:
===========================================================================
	1. Authentication for API
	2. Action filters for logging request/response
	3. Exception logging logic into custom created Action Filter 
	 
