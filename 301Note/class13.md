## Class 13 Reading Notes: CRUD

#### CRUD Basics

1. Which HTTP method would you use to update a record through an API?
  - PUT - this replaces all current data of the targeted resource with new data using an id
  - CRUD corresponds the the HTTP methosd
2. Which REST methods require an ID parameter?
  - delete and put require an id to know which resoures is being targeted

#### Videos

**Speed Coding: Building a CRUD API (Watch a Twitch streamer code an Express API in 20 minutes!)**

1. What’s the relationship between REST and CRUD?
  - rest and crud work in sync. Rest is a way to manage data communication between APIs and crud is a way to manage how the data is manipulated
  - REST is an archetectural style used to share data between web-servers. CRUD is the basic functionality of an API that is used to manipulate data. CRUD functions exist in RESTful APIs to provide the foundational functionality of an API.
2. If you had to describe the process of creating a RESTful API in 5 steps, what would they be?
  1. Create Routes for get, post, put, and delete
  2. create schema and model
  3. Create objects that align with schema requirements and use post to send to database 
  4. Use Get request to grab data from database using object id to select specific items
  5. Using the id from url, request to delete and update database