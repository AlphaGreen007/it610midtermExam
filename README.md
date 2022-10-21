# it610midtermExam
IT610 Midterm Exam Repository for Thomas H.

Welcome to Thomas' userguide for the it610 Midterm Exam!

Deliverable: Create a docker container with a MySQL instance.

ROOT PASSWORD: openproject
***********************************************************

STEP 1: Type the following Powershell command. Include the period.  Feel free to change 'midtermExam' to another random name:

docker build -t midtermExam .  

STEP 2: Run the midtermExam image with the following PowerShell Command to initialize the container:

docker run --name midtermExam -d -e MYSQL_ROOT_PASSWORD=openproject mysql:latest

STEP 3:  Interact with the midtermExam container with the following Powershell command:

docker container exec -it midtermExam bash

STEP 4: Now that we are able to interact with the mySQL container, we can execute mySQL commands inside of it with the following Powershell command:

mysql -uroot -popenproject

STEP 5: List all of the databases within the container with the following command:

show databases;

CONGRATULATIONS, you have completed the tutorial for creating one instance of a docker container that uses a   MySQL application.
