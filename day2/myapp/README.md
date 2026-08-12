Generate:

Basically generate automatically create the rails file structure and folder structure instead of manually add the file and folder it's follow the rails default naming convention.

Model View Controller (MVC)

In MVC structure the file follow the require structure

. Model

Models manage data and business logic. Main use of model is model interact with the database, validate the data and define the relationships.
Example:
class User < ApplicationRecord
end

Location:

app/models/

. View

Views are responsible for displaying information to users.

Location:
app/views/

. Controller

Controllers handle user requests and connect Models with Views. Main work of the controller is it's receive the requests, fetch the data from the models, send data to the views

Location:
app/controllers/
