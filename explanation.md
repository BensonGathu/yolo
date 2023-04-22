I choose node:bullseye-slim image for both containers beacause of its size and security features.
Added a maintainer label to the Image
Using WORKON i created a directory named /MyApp where my code would be stored
COPIED packages.json from my current to my new working directory "MyAp"
Using "RUN npm install" I installed the required packages for the app to function accordingly
Then Copied all other files to my working Directory
Exposed port 5000 which will be used by the application.

Using "CMD [ "npm", "start"]". When the container starts the commands npm start will be run.


