I choose node:bullseye-slim image for both containers beacause of its size and security features.
Added a maintainer label to the Image
Using WORKON i created a directory named /MyApp where my code would be stored
COPIED packages.json from my current to my new working directory "MyAp"
Using "RUN npm install" I installed the required packages for the app to function accordingly
Then Copied all other files to my working Directory
Exposed port 5000 which will be used by the application.

Using "CMD [ "npm", "start"]". When the container starts the commands npm start will be run.


Added playbook.yml file where my ansible books will be written
Inside the playbook we have three roles (Git,Docker,compose)
Git will handle the following tasks. 
1. install git
2. Clone our repository
Gocker will have the following tasts
1. install and ensure docker is installed and running
2. install docker-compose
compose will ensure the docker compose up is ran on our docker-compose.yml file.
