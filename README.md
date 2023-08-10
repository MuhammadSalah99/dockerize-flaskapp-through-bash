# This is my code for the second Task 


I used docker-compose.yaml to build and run multiple images and thier containers.

### To Run use ```/spin-up.bash admin admin db``` 

Note you might need to run ```cmmod +x ./spin-up.sh``` to make the scipt excutable

it will be running on [http://localhost:5000](http://127.0.0.1:5000)

## This was my approach for the first opption for Task 2,

I wanted to try out bash with the docker build commands, so I wrote this bash file to help us manage and spin up our containers without much of a hassle.

1. I created a Dockerfile with all the configurations to set up flask.
2. I uploaded my image to [dockerhub](https://hub.docker.com/repository/docker/muhammadssalah99/flask-ecs-terraform), so anyone can use it with the script. 
3. I created a bash file, with 3 varibles, the first Postgres password, the second Postgres user and finally Postgres databse.
4. I took this step because its more secure and safe than having it hardcoded in the ```docker build``` command. 
5. Then I check if the network that we need to use between our containers exits, if not create it 
6. after then I make sure that the db container is not running or doesnt exist, just in case
7. then I excecute my build commands


this is a simple and scalable approach for Dockerizing our flask app.


