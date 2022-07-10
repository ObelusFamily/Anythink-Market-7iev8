# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

This section will describe the first setup needed to get all the code and run it on your computer
### Cloning the repo
Its important to **clone** that repository, before doing any other tasks.
You can do it by using the following command (assuming that you have git command line tools installed): 

```git clone https://github.com/ObelusFamily/Anythink-Market-7iev8.git```


### installing a docker

So first thing’s first - install Docker: [follow instructions](https://docs.docker.com/get-docker/).

You can verify docker is ready by running the following commands in your terminal: 
```docker -v``` 
and 
```docker-compose -v```.

### Running and testing the docker
From the project root directory, run: 
```
docker-compose up 
```
to load Anythink's backend and frontend.

If docker is working correctly, the backend should be running and able to connect to your local database. Let's test this by pointing your browser to http://localhost:3000/api/ping

To check the frontend and make sure it’s connected to the backend, create your username and password at : http://localhost:3001/register.
If everything is ok, you'll see a blue background.

Make sure that you run all scripts on one of the containers created by docker-compose up.  You can use docker exec to run commands on a running container.
