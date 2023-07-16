# Akademi2023

1- The application code was downloaded, and a repository named "akademy2023" was created on GitHub.

2- A Dockerfile was created to containerize the application, and this Dockerfile was pushed to the created Git repository.

3- An image repository was created on Docker Hub to store the generated Docker image.

4- The application was run locally, and when a request was made, it was observed that the "BC4M" message appeared, indicating that the application was running.

#### Commands used to push code to a Git repository
 
    git init
    git add .
    git add -m "akademi2023"
    git commit -m "akademi2023" 
    git main

#### Commands used to push code to a Git repository

   docker build -t akademi2023 .

#### Commands used to push a Docker Image to Docker Hub image repository

   docker tag akademi2023 ensarkol/akademi2023:latest
   docker image push ensarkol/akademi2023:latest
   
#### Commands used to run and test the application

  docker pull ensarkol/akademi2023:latest
  docker run -d -p 5000:5000 ensarkol/akademi2023:latest
  curl localhost:5000
