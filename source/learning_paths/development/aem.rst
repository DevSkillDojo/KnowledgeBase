.. _aem:

Learning Path :: Development : AEM
==================================

Note: This learning path is still under development. If you would like to add any details, references or ideas, please submit a pull request

* Overview of AEM
   * Why does AEM exist?
   * What are the competitors in the market
   * The core technologies in AEM
   * The roles on an AEM project 
      * Project Manager
      * Architect
      * Business Practitioner
      * Author
      * Tester
      * Back-End Developer
      * Front-End Developer
      * Integration Developer
      * Systems Engineer

* Prerequisite Background Knowledge (Project Manager)
   * TODO
    
* Prerequisite Background Knowledge (Architect)
   * :ref:`Git <skills_detail_git>` (4 - Advanced) 
   * :ref:`HTML5 <skills_detail_html5>` (3 - Intermediate)
   * :ref:`JavaScript <skills_detail_javascript>` (3 - Intermediate)
   * :ref:`CSS3 <skills_detail_css3>` (3 - Intermediate)
   * :ref:`JQuery <skills_detail_jquery>` (3 - Intermediate)
   * :ref:`Java <skills_detail_java>` (4 - Advanced)
   * :ref:`Maven <skills_detail_maven>` (4 - Advanced)
   * :ref:`Apache httpd <skills_detail_apache_httpd>` (3 - Intermediate)
   * TODO

* Prerequisite Background Knowledge (Business Practitioner)
   * :ref:`Git <skills_detail_git>` (2 - Novice)
   * TODO

* Prerequisite Background Knowledge (Author)
   * TODO
    
* Prerequisite Background Knowledge (Tester)
   * :ref:`Git <skills_detail_git>` (3 - Intermediate)
   * TODO    

* Prerequisite Background Knowledge (Front-End Developer)
   * :ref:`Git <skills_detail_git>` (3 - Intermediate)
   * :ref:`HTML5 <skills_detail_html5>` (3 - Intermediate)
   * :ref:`JavaScript <skills_detail_javascript>` (3 - Intermediate)
   * :ref:`CSS3 <skills_detail_css3>` (3 - Intermediate)
   * :ref:`JQuery <skills_detail_jquery>` (2 - Novice)
   * :ref:`Java <skills_detail_java>` (2 - Novice)
      * Java logging (1 - Fundamental Awareness)
      * TODO
   * :ref:`Maven <skills_detail_maven>` (2 - Novice)
   * :ref:`Apache httpd <skills_detail_apache_httpd>` (2 - Novice)
   * :ref:`TLS/SSL <skills_detail_tls_ssl>` (1 - Fundamental Awareness)
   * :ref:`Docker <skills_detail_docker>` (2 - Novice) (For local environment prep)
   * :ref:`Docker Compose <skills_detail_docker_compose>` (2 - Novice) (For local environment prep)  
   * :ref:`JSON <skills_detail_json>` (2 - Novice)
   * :ref:`Bootstrap <skills_detail_bootstrap>`  (3 - Intermediate) (Not sure if this is really true)
   * IDE
   * Eclipse
    
* Prerequisite Background Knowledge (Back-End Developer) 
   * :ref:`Git <skills_detail_git>` (3 - Intermediate)  
   * :ref:`HTML5 <skills_detail_html5>` (2 - Novice)
   * :ref:`JavaScript <skills_detail_javascript>` (2 - Novice)
   * :ref:`CSS3 <skills_detail_css3>` (2 - Novice)
   * :ref:`JQuery <skills_detail_jquery>` (2 - Novice)
   * :ref:`Java <skills_detail_java>` (3 - Intermediate)
      * Java logging (3 - Intermediate)
      * Java Servlets (3 - Intermediate)
      * Java Dependency Injection (3 - Intermediate)
      * JMX (3 - Intermediate)
      * JAAS (3 - Intermediate)  
      * Spring rest services (3 - Intermediate) (Because you are almost 100% certain to have to build some service that AEM can consume)
      * OSGi (3 - Intermediate)
      * TODO
   * :ref:`Maven <skills_detail_maven>` (3 - Intermediate)
   * :ref:`Apache httpd <skills_detail_apache_httpd>` (2 - Novice)
   * :ref:`Docker <skills_detail_docker>` (2 - Novice) (For local environment prep)
   * :ref:`Docker Compose <skills_detail_docker_compose>` (2 - Novice) (For local environment prep)    
   * James mail (2 - Novice) (For local email dev)
   * Ldap (2 - Novice)

   * Testing HTTP endpoints with Postman (3 - Intermediate)
   * JSON (3 - Intermediate)
   * SQL (3 - Intermediate)
   * IDE
   * Eclipse
 
* Prerequisite Background Knowledge (Integration Developer) 
   * :ref:`Git <skills_detail_git>` (3 - Intermediate) 
   * IDE
   * Eclipse
   * TODO
   
* Prerequisite Background Knowledge (Systems Engineer)
   * :ref:`Git <skills_detail_git>` (3 - Intermediate)
   * IDE
   * Eclipse
   * TODO    
    
* Beginner topics
   * Setting up the core prerequisites (JDK, Maven)
   * Starting up AEM for the first time
   * Overview of AEM interfaces
   * Exploring the Felix console
   * Exploring CRX DE
    
* Beginner Project 1 - Your first AEM project
   * Goal: Understanding Sling routing
   * Create Git repo
   * Create your own application with Maven
   * Basic Sling UI with Sightly (Catalogue-type site)
   * Pull request
   
* Beginner Project 2 - Introducing the JCR
   * Goal: Get familiar with the JCR and how to work with it  
   * Structure of the AEM JCR (What goes in the different folders)
   * Working with data using CRX DE
   * JCR Queries from CRX DE

* Beginner Project 3 - SlingPostServlet
   * Goal: Use SlingPostServlet to add data to the JCR
   * Create a set of Postman requests for adding data into the JCR
   * Pull request

* Beginner Project 4 - Our own servlet
   * Goal: Add some stand-alone OSGi services and a servlet to access it
   * Architecture layers -> Servlets call services
   * GET Method
   * POST Method
   * PUT Method
   * DELETE Method
   * OSGi Service with relevant methods
   * Create a set of Postman requests to call our servlet
   * Pull request

* Beginner Project 5 - Interacting with the JCR
   * Goal: Connecting to the JCR from Java
   * Adding, Reading, Updating and Deleting nodes to the JCR (in service)
   * JCR Queries from Java
   * Test using Postman
   * Pull request
   
* Beginner Project 6 - Sling models
   * Goal: Understand how Sling models are used to provide back-end data for the front-end
   * Build Sling model with a Read Only screen
   * Add an "Edit mode" for the screen
   * Add a "Create mode" for the screen
   * Add servlet interactions for Create, Update and Delete operations
   * Pull request
   
* Beginner Project 7 - Polishing up
   * Goal: Some final clean-up of the project
   * Adding base content from ui.content
   * Summarise where content from the source code is deployed
   * Look at our package in the CRX Package Explorer
   
* Beginner Project 2 - Setting up a full(ish) environment
* Beginner Project 2 - Preparing an LDAP server with docker
* Beginner Project 2 - Adding LDAP login to AEM
* Beginner Project 2 - Adding SSL to AEM
* Beginner Project 2 - Adding a Dispatcher
* Beginner Project 3 - Creating authorable components
* Beginner Project 3 - Understanding the role of the author vs the developer
* Beginner Project 3 - Creating Page templates
* Beginner Project 3 - Allowing authors to create pages
* Beginner Project 3 - Authoring pages with OOTB components
* Beginner Project 3 - Controlling what authors can do an a page
* Beginner Project 3 - Controling what pages authors can create
* Beginner Project 3 - Creating a navigation bar component in sightly
* Beginner Project 3 - Publishing authored content
* Beginner Project 4 - Tools of the Trade
* Beginner Project 4 - Eclipse AEM tools. Push and pull from AEM
* Beginner Project 4 - Brackets for easy UI synching
* Beginner Project 4 - VLT
* Beginner Project 4 - Configuring VLT filters
* Beginner Project 4 - BND and the Maven Bundle Plugin
* Beginner Project 4 - Understanding the Adobe profiles in Maven
* Intermediate Project 1
* Intermediate Project 2 - ACS Commons
* Intermediate - Osgi - Karaf book
* Intermediate - Request processing in Sling
* Intermediate - Vanilla Sling application
* Intermediate - Vanilla Jackrabbit application
* Intermediate - AEM Email service
* Intermediate - Servlet filters
* Intermediate - JCR versioning
* Intermediate - JCR permissions
* Advanced - Adding checkstyle to your project
* Intermediate - Configuring Dispatcher caching


Vanilla Apache Sling
--------------------
The steps described below would be very useful if combined in a GitHub-driven video series

* Download and run sling
* Content and apps using curl and resource explorer
* Mvn content project
* Mvn bundle project
* Setting up eclipse to connect to sling
* Building a servlet
* Building an OSGI component that interacts with the JCR
* Putting the serlvet and osgi componenet together. Using postman to call it
* Adding an HTL front-end
* Using a sling model with the HTL feont end
* Setting up easy front end code synch solution (visual studio code) ?
* Setting up vault
* Adding a scheduler
* JCR indexing
* Integration testing
* Adding configurations




* Beginner - WKND tutorial (Not sure where this should fit in)




















