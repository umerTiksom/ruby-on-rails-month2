1. What is Ruby on Rails?

   Ruby on Rails is an open-source web application framework written in the Ruby programming language. It supports MVC architecture that provides a default structure for database, web pages, and web services, it also uses web standards like JSON or XML for transfer data and HTML, CSS, and JavaScript for the user interface. Rails provides a set of tools, libraries, and conventions that help developers focus on business logic instead of writing repetitive configuration code. It is widely used for creating websites, APIs, e-commerce platforms, management systems, and SaaS applications.

2. Rails Philosophy

   Rails tries to reduce unnecessary decisions, repetitive code, and configuration so developers can focus on building the actual application.
   Rails is based on two important principles:

   . Convention over Configuration (CoC)
   Rails follows predefined conventions. Developers do not need to configure everything manually.
   Example:
   A model named User automatically maps to a database table named users.Controller names and file locations follow standard naming conventions.This reduces development time and keeps projects organized.
   . Don't Repeat Yourself (DRY)
   Rails encourages developers to avoid duplicate code.Instead of writing the same logic multiple times:
   Use methods
   Use helpers
   Use partials
   Reuse components
   This makes applications easier to maintain and update.
   For example, imagine you have:
   def create_user
   puts "Operation completed successfully"
   end
   def update_user
   puts "Operation completed successfully"
   end
   The same information is repeated.
   If you need to change the message later, you have to update multiple places.
   A better approach is to put common logic in one reusable place.

3. MVC Architecture

   Rails follows the MVC (Model-View-Controller) pattern.
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

4. Rails Directory Structure

   Rails folder structure are as follow:

   app/

   This folder contain the main application code. This folder constain the main MVC structure and you mostly work on this folder.

   config/

   This folder contain all the configuration of your application routes, database etc.

   db/

   This folder contains database-related files and database migrations.

   bin/

   This folder contains all the scripts for start, set up and deploy your application .

   lib/

   Contains custom modules and reusable code.

   public/

   This folder contain the static files.

   storage/

   Used for uploaded files with Active Storage.

   test/

   Contains automated tests and the models test files.

   Gemfile

   Lists all project dependencies (gems).
   Example:
   gem "rails"
   gem "pg"
   gem "puma"

5. Five Important Observations from Exploring a Generated Rails Application

   Observation 1

   Rails creates a complete project structure automatically so that we are not creating it manual

   Observation 2

   The app/ directory contains most of the code related to business logic, views, and controllers.

   Observation 3

   Routing is centralized in config/routes.rb . All URLs are managed from one location.

   Observation 4

   Database changes are managed using migrations inside db/migrate/ .This allows version control of the database structure.

   Observation 5

   Rails follows strong conventions which means developers can easily understand and work on different Rails projects because the structure remains consistent.
