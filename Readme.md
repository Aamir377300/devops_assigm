virtual environment is created using python3 -m venv venv

and activate it source venv/bin/activate

contontorization is done using the 

docker build -t flask-app .
docker run -p 5005:5000 flask-app

and it running on teh port --> http://localhost:5005/

and contorization id is 192.168.65.1

-----------------------

building the docker after adding the .github/workflow

docker build . --file Dockerfile --tag flask-app:latest

run the container 
docker run -d -p 5005:5005 --name flask-app-container flask-app:latest

450ebeaf59a73287b245bf3486d639116bfc8b5af38dd91be6ceea10dd2eaa75


-----------------------------------



if i change the anything in the app.py so i have again build the image and run the container due to i deploy on the locally 

the url in which this run :-> http://localhost:5005/


---

automatic rebuild 

docker compose watch
