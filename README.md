## Title of Project
MediYantra Health Service - A suitable website to offer basic health services

## Desciption
MediYantra is a cloud-enabled, mobile-ready Express JS powered web application to help people .

## Software Requirements
  - NodeJs
  - MongoBD
  - MySQL
  - HTML & CSS
  - Google Maps API
  - elfsight Website Widgets
  
## Process Flow

## Data Flow Diagram

## Installation

MediYantra requires [Node.js](https://nodejs.org/) v4+ to run.

Install the dependencies and devDependencies and start the server.

```sh
$ git clone https://github.com/darkpanda08/MediYantra-Heath-Service.git
$ cd MediYantra-Heath-Service
$ npm install
$ npm run start
```
For development environments...
```sh
$ npm run dev
```
For production environments...

```sh
$ npm run start
```
Note: If the application is being run other than on localhost, HTTPS is mandatory to use Geolocation feature.

### Extra Steps to Perform 

MediYantra is currently extended with the following tools. Instructions on how to set them up are mentioned below.

1) To setup MongoDB, get the URI for MongoDB and paste it in config/keys.js file inside the quotes on line 2.

2) To setup MySQL, Create a database and provide the connection details as envronment varibales as below mentioned:
DB_host : Hostname
DB_user : Username
DB_pass : Password
DB_name : Database Name

3) Create three tables as below mentioned in the above created database.
(a) helpline_details : With columns id, uid, first_name, last_name, qualification, speciality, hospital, location, email and telephone.
(b) ngo_details: With columns id, name, website and phone 
(c) testing_centres: With columns id, state and name

4) Go to elfsight.com and create 4 widgets: Click to call, Social Media links, Chats and Coronavirus Track and add the provided code into the views/dashboard.ejs in line 89 and views/layout.ejs in line 17-19.

