# DisasterAlleviationFoundationAPPRFINAL
App flow:
- Home Page (Index):
   -Navigation:
    -Register/Login - Profile edits
    -Volunteer : Register as volunteer
    -Admin login - Manage volunteer and volunteer tasks
    - Donation - submit donation
    - Disaster - report disaster (details)

Explaination of models: 
In this application, models in C# (classes in the Models folder) represent the structure of the data we work with in the code. Each model corresponds to a database table in Azure SQL:

Properties of a model (like DonorName, ResourceType, Quantity in the Donation model) map to columns in the table.

When the application runs, Entity Framework Core uses these models to create, read, update, and delete records in the database.

Changes to the model structure (adding/removing properties) are applied to the database via migrations, keeping the code and database in.

##PART 3 UPDATES:##
Testing phase and deployment,
- The rest of this project contains testing to allow for the deployment of the application on azure web app.
- This project contains:
- Unit tests = testing of models
- Integration tests = testing on controllers and database integration connections
- UI tests = testing of user interfaces *views*
- As well as load tests and stress testing using apache jmeter
- and automated testing to allow final deployment
