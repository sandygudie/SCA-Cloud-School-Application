# SCA-Cloud-School-Application
  Creating a Dockerfile with Node js

### Running the project locally
- Fork this repository
- Clone to your local machine and `cd` into the repository.
- Checkout to the branch `stable` from master branch
- Run `npm install && npm start`
- Go to http://localhost:8080
- A welcome message "Welcome to SCA Cloud School Application" will show on the browser.


### Deploy Stable branch to Docker hub
- Open An account with Docker hub [docker.com] and download the docker desktop
- To build Docker image - Type  `docker build -t dockerdemo .` 
- To run the Docker image - `docker run -p 49160:8080 -d dockerdemo`
- Run the image on your Docker desktop, you should have the welcome message.

### Feature Branch
- Checkout to feature branch.
- Build Docker image - Type  `docker build -t docker-feature .` 
- Run the Docker image - `docker run -p 4990:8080 -d docker-feature`
- Run the image on your Docker desktop, you should have the welcome message. "Welcome to SCA Cloud School Application , this is my first assessment"

### See Docker images and id
- Run `docker images`

### Push to docker repo
- Create a repo in docker hub, my repo name:sca-cloud-docker
- Run `docker tag image-id:yourhubusername/reponame:tag` (docker tag 9c9f09c6e82e yourhubusername/sca-cloud-docker:stable)
- Run `docker push yourhubusername/reponame:tag` (docker push yourhubusername/sca-cloud-docker:stable)
- Did same for feature branch in the same repo


### Pull Images
- `docker pull sandy8169/sca-cloud-docker`

### Docker Hub Repo
- sca-cloud-docker
 
