.. _basic_survey_system:

Learning Project: Basic Survey System
=====================================

Introduction
------------

What are learning projects:
* The purpose of learning projects is to allow learners to build a real-world solution in a guided manner, but without the detailed
step-by-step instructions that are typically found in online tutorials. 
* Instead, the solution expectations are described and the learner needs to find there own way.

If you get entirely stuck, the source code for each stage of the project is available on the GitHub project

Level: Beginner/Intermediate
* This learning project is designed from the ground up to assist the learner with assembling a full solution based on multiple components.
* It is assumed that the learned has used most of the component solution technologies in isolation, but still need better guidance in how to use them together

The project may later be extended into a series which will improve the front-end capability 

The technology that will be used are:
* Git and GitHub
* MySQL database
* SpringBoot (Java) Service
* Postman
* JUnit
* TBD - Jackson
* TBD - Hibernate (Perhaps pure JDBC)
* TBD - Maven
* HTML5 + CSS3 Front-End
* JQuery
* Your favourite Java IDE

The table below provides some useful learning resources for each of the skills that will be used in this project:

+---------------+-------------------+----------------------+
| Technology    | Proficiency Level | Learning Resource(s) |
+===============+===================+======================+
| HTML5         |                   |                      |
+---------------+-------------------+----------------------+
| CSS3          |                   |                      |
+---------------+-------------------+----------------------+
| JavaScript    |                   |                      |
+---------------+-------------------+----------------------+
| JQuery        |                   |                      |
+---------------+-------------------+----------------------+
| Java          |                   |                      |
+---------------+-------------------+----------------------+
| SpringBoot    |                   |                      |
+---------------+-------------------+----------------------+
| REST Services |                   |                      |
+---------------+-------------------+----------------------+
| SQL           |                   |                      |
+---------------+-------------------+----------------------+
| MySQL         |                   |                      |
+---------------+-------------------+----------------------+
| Hibernate     |                   |                      |
+---------------+-------------------+----------------------+
| Maven         |                   |                      |
+---------------+-------------------+----------------------+
| Jackson       |                   |                      |
+---------------+-------------------+----------------------+
| JDBC          |                   |                      |
+---------------+-------------------+----------------------+
| Git           |                   |                      |
+---------------+-------------------+----------------------+
| GitHub        |                   |                      |
+---------------+-------------------+----------------------+
| Postman       |                   |                      |
+---------------+-------------------+----------------------+
| JUnit         |                   |                      |
+---------------+-------------------+----------------------+
|               |                   |                      |
+---------------+-------------------+----------------------+



Solution Overview
-----------------
The solution that we will be building is a very simplistic survey system that will allow end users to capture a submission 
for a survey, view a list of submissions and also view the details of other submissions. This type of system may be used for various
purposes, but in our case, let's assume it will be used by an insurance company who received policy applications, adjustments and claims
from their customers.

The diagram below provides an overview of the screen flow that will be created:

TODO - Add screen flow. Pretty much breadboards of what we will be building

To make the solution as simple as possible, the following functionality is excluded from scope:

* Login, i.e. the app will be open to unauthenticated users. This means everybody will be able to see everyubody else's submissions
* Editing a form after it has been submitted
* Multiple forms, i.e. the initial solution will contain only one form

Stage 1 - Create a new git repo
-------------------------------
Every project begins with a Git repository. We will be using GitHub for hosting our repository.

Goals for stage 1:
* Fork your base repository on GitHub (Base repo URL would've been sent to you on registration to this module)
* Clone the repo to your local machine.

Stage 2 - Building a screen for our first form
----------------------------------------------
Although the system will be designed to handle multiple form types, we need to start with one. 

As they say: A journey of a thousand miles begins for a first step.

Our first form will be a very basic short term insurance quote request form. It allows you to request a quote for homeowners insurance.

The fields that should appear on the form are:
* Customer Name
* Customer Surname
* Customer Id, Passport or Social Security number
* Physical address line 1
* Physical address line 2
* City
* State or Province
* Country
* Postal code
* Property value amount (in USD)

TODO - Details to follow

Goals for stage 2:
* In the repo, create a folder called src/web
* Create a new file for our form called "basic-claim.html"
* Create an HTML form, with a single submit button on the html page
* Commit and push your changes to git
* Send a Pull Request

If you get stuck, feel free to look at the reference implementation here: TODO 

Stage 3: SpringBoot Service method (POST)
-----------------------------------------
The next step is to build a SpringBoot POST method to which the form data will be submitted. For now we will
NOT be saving the data to a DB, we will only log it to the system log.

Notes:
* Still just submit dummy data into the payload field
* Use Postman to test first

TODO - Details to follow

Goals for stage 3:
* TODO

If you get stuck, feel free to look at the reference implementation here: TODO 

Stage 4: Link the HTML front-end button with POST service
---------------------------------------------------------
TODO - Details to follow

Stage 5: Create a Database using a DDL script
---------------------------------------------
In-line with our goal for simplicity, the initial database will comprise a single table. The table will contain one row for each
submitted return. Note: We will be calling each submitted survey a RETURN, so the table will be called Returns

The table will have the fields listed below:

+-------------+-----------+----------------------------------------------------------------------------------------------+
| Field Name  | Data Type | Description                                                                                  |
+=============+===========+==============================================================================================+
| ReturnId    | UUID      | A universally unique id for the the return                                                   |
+-------------+-----------+----------------------------------------------------------------------------------------------+
| FormType    | String    | A reference to the type of form that was submitted.                                          |
+-------------+-----------+----------------------------------------------------------------------------------------------+
| DataPayload | String    | All the data that was captured in the form, stored as a single JSON string encoded as Base64 |
+-------------+-----------+----------------------------------------------------------------------------------------------+
| Timestamp   | DataTime  | The exact moment in time when the return was submitted                                       |
+-------------+-----------+----------------------------------------------------------------------------------------------+

Instead of building this table using a GUI of some sort, we will create SQL DDL script which describes the DB table.
This script can then easily be executed against a database to produce the database according to our needs.

Goals for stage 5:
* In the repo, create a folder called "database"
* In this folder, create a SQL DDL script called "create_db.sql"
* Create a SQL statement that will create the table as described above

If you get stuck, feel free to look at the reference implementation here: TODO 

Stage 6: Link SpringBoot service to DB
--------------------------------------
TODO - Details to follow

Notes:
* Base64 encoding of the form payload

Stage 7: Add a SpringBoot service for getting all returns
---------------------------------------------------------
TODO - Details to follow

Notes:
* Test with Postman

Stage 8: Add screen for showing all returns
-------------------------------------------
TODO - Details to follow

Notes:
* JQuery to build page at runtime

Stage 9: Add SpringBoot method for getting details of one return
----------------------------------------------------------------
TODO - Details to follow

Notes:
* Base64 decoding of the form payload
* Test with Postman

Stage 10: Add screen for displaying a return as read-only
---------------------------------------------------------
TODO - Details to follow

Stage 11: Add index page
------------------------
TODO - Details to follow

Stage 12: Style all pages consistently
--------------------------------------
TODO - Details to follow


Ideas for further improvement
-----------------------------
As mentioned earlier, this application was kept simple on purpose. However, there are many ways in which we can improve on it.
These improvements will be explored is future bolt-on project, but are listed here for the reader's interest:

* Add user registration and login
* Store information about which user submitted each form. A user should only be able to see their own forms
* More impressive front-end using a modern front-end framework like React
* Adding multiple form types
* Downloading a PDF version of your submitted form
* Getting an email confirmation once a form is submitted
* Allow users to add attachments to forms
* Refactor the SpringBoot application to use proper Services
* Add server-side validations
* And much more

Project Development Notes:
--------------------------
 * The flexibility of a document-based DB may be preferable here. Perhaps a Mongo instead of a MySQL DB
 * Learners should submit a pull request for format review, but this requires that they fork a base repo
 * Test the solution with Senior engineers

