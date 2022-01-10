# workshop2
 Django Tutorials application and deploy it to your AWS EC2 instance, so that it is accessible over the internet and not just on your own computer.
You will also set up a cloud-based Postgres database for the Tutorials application, using the AWS Relational Database Service (RDS).
In this concept it is very important to understand: The EC2 instance is not on your computer.
You access it from your computer through a SSH session, but what you are accessing is a completely different computer that exists somewhere else in the world, that you connect to through the internet.
If you run into issues on the EC2 server because you made a mistake on a file there, such as the docker-compose.yml or the settings.py file, you CANNOT fix this error by updating your local version of that file. It is not the same file! Changes you make in VS Code on your computer do not affect anything on the EC2 server! 
If you need to update a text file on the server, you must use a text editor on the EC2 server, such as vi or nano.
 First you need to Launch an EC2 Instance, Configure Amazon Web Services, and Set Up Your EC2 instance, in that order. 
Then,create RDS database in AWS console. The RDS is Amazon's cloud-based database management service, which can run PostgreSQL database servers along with other popular options.
 Set up the Django application for deployment.
 Clone repository on EC2 instance, build and run Docker application, apply migrations.
 Make and apply the migrations inside the Docker container.
 Open Insomnia and create a new POST request.
For the URL, use http:// followed by your EC2 instance DNS address, followed by :8000/api/tutorials/.
