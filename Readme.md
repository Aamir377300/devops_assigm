building the docker after adding the .github/workflow

docker build . --file Dockerfile --tag flask-app:latest

run the container 
docker run -d -p 5005:5005 --name flask-app-container flask-app:latest


-------------------------------

Automatic rebuild is done using the compose and also ci/cd is added

we going to use the compose concept 

and run it -->  docker compose up --build


and stop it --> docker compose down

now the live reloading is take place 

/////

setup 

git clone https://github.com/Aamir377300/devops_assigm.git

cd devops_assigm

then run the compose

docker compose up --build

port --> http://localhost:5005/

to stop --> docker compose down
