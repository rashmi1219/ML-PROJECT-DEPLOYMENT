# ML-project-deployment
this a ml project with full CICD
######
start machine learning project
software and account requirements
1. [Github Account](https://github.com)
2. [Heroku Account](https://dashboard.heroku.com/login)
3. [vs code IDE](https://code.visulastudio.com/download)
4. [GIT cli](https://git-scm.com/downloads)
5. [GIT Documentation](https://git-scm.com/docs/gittutorial)

```
create environment
conda create -p venv python==3.7 -y
```


```
activate conda environmet
conda activate venv
      or
conda activate venv/
```
```
create requirements.txt file
pip install -r requirements.txt
```
```
create app.py file
if file is not running or there is some problem with flask installation error 
please set anaconda environment variable
```
```
add file to github for version control(vcs)
if individual file is to be added
git add file1 file2
     or
if all the files present in current directory has to be updated
the command is.
git add .

if any file is not updated in git we can check it with command
git status
if file is not updated it will show some kind of error

if we have to create version in git we use commit command
git commit -m "message"
      and
if we want to see all the existing version the command is
git log

to send version to github command is
git push origin main

to check remote url command is
git remote -v
```
```
difference between get and post methods
GET:here the information will be sent to browser through url
POST:information will be encrypted will be sent through body so that one one can see those information
```
to create CICD pipeline in Heroku we need three information
1. Heroku email id
2. Heroku API key :6a02c0bc-327f-4eec-94a1-5459dae2aa96
3. Heroku APP name:ml-regression-project7

```
create a dockerfile
Dockerfile
```
```
add one gunicorn library to requirements.txt file
```
```
now we need to write some instruction in docker file to create docker image
FROM python:3.7

create one more file which will ignore those file which is not needed
.dockerignore(we will mention file like venv/, .git, .gitignore)
now we have to copy all the file and folder in current dir to docker file command is
COPY ./app





```
```
BUILD DOCKER IMAGE
docker build -t <image_name>:<tagname> .
note:image name for docker will always be in lower case

To list docker image command is
```
docker images

```
run docker image
```
docker run -p 5000:5000 -e PORT=5000 <image_id>
```
to check running dicker container command is 
```
docker ps
```
to stop docker container command is
```
docker stop <container_id>

```
create a new folder
```
.github

```









