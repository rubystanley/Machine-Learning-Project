## Start Machine-Learning-Project

#### Software Requirements

1. [VS Code](https://code.visualstudio.com/download)
2. [GitHub Account](https://github.com)
3. [Heroku Account](https://dashboard.heroku.com/login)
4. [GIT CLI](https://git-scm.com/downloads)
5. [GIT documentation](https://git-scm.com/docs/gittutorials)

Creating conda environment
...
conda create -p venv python==3.7 -y
...
Activate conda environment
conda activate venv-

Create requirements.txt file
pip install -r requirements.txt

To add files to git

git add . 

or

git add <filename>

Note : To ignore file or folder from git we can write name of file/folder in .gitignore file

To check the git status 
...
git status
...

To check all version maintained by git
....
git log
....

To create version/commit all changes by git
...
git commit -m "message"

To send committed changes to github
..
git push origin main
...

To check origin/remote url
...
git remote -v
...

To set up CI/CD pipeline in Heroku we need 3 information . Heroku api key is from top left account setting
1. HEROKU_EMAIL = rubystanley@gmail.com
2. HEROKU_API_KEY =<>
3. HEROKU_APP_NAME=ml-regression-app86

BUILD DOCKER IMAGE
...
docker build -t <image_name>:<tagname> .
...

Note : Image name for docker must be lowercase

To list docker image 
...
docker images
...

Run docker image
...
docker run -p 5000:5000 -e PORT=5000 <imageid>

check localhost:5000 to see if the app is working

...
TO STOP DOCKER CONTAINER

TO CHECK RUNNING CONTAINERS
..
docker ps
...


To stop docker container
...
docker stop <container_id>
...