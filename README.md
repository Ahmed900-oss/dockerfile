Step 1: Create a Simple Application
For this example, we’ll create a straightforward Node.js application. Create a directory for your project and navigate to it in your terminal.
Inside your project directory, create a simple app.js file
This basic Node.js application sets up a web server that responds with “Hello, Docker World!” when accessed.

Step 2: Create a Dockerfile
A Dockerfile is a script that defines the instructions to build a Docker image. Create a file named Dockerfile (no file extension) in your project directory
This Dockerfile sets up a Node.js environment in a container, copies your application code and dependencies, and specifies how to run the application.

Step 3: Build the Docker Image
With your Dockerfile in place, you can build a Docker image for your application. In your project directory

docker build -t my-docker-app .
The -t my-docker-app option tags the image with the name "my-docker-app" for easier reference.

Step 4: Run the Docker Container
Now that you have built your Docker image, you can run a Docker container from it. Use the following command.

docker run -p 3000:3000 my-docker-app
This command maps port 3000 in the container to port 3000 on your host machine, allowing you to access your application in a web browser.

Step 5: Access Your Dockerized Application
Open your web browser and navigate to http://localhost:3000. You should see "Hello, Docker World!" displayed, indicating that your Dockerized application is running successfully.
