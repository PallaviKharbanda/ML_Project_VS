# ML_Project_VS


Software Requirements :

[github account](https://github.com/) 

[git cli](https://git-scm.com/downloads)

[vs code](https://code.visualstudio.com/)

[Heroku Account](heroku.com) 



Creating  and  Activating virtual environment
```
conda create -p venv python==3.7 -y # -p to create venv in project folder itself so that we can delete it altogether
conda activate venv or conda activate venv/
```
Installing necessary files

```
pip install -r requirements.txt
```

Cloning Repository
```
Create a repository on github and clone it on local using:

git clone https://PallaviKharbanda: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@github.com/PallaviKharbanda/ML_Project_VS.git

(For a particular path location, first create a folder and then use cd that folder location and then use git clone command)

use code . to open visual code from terminal(To enable this command, open VS app, type Command+shift+P and typr install shell command so that code . is successfully opened from command)

```
From local to github repository
```

git add <folder1> <folder2> <etc.> #git status, git log to see all versions
  
git commit -m "Your message about the commit" #for commiting

git push origin main # For pushing the code
```

To set up CI/CD Pipeline in Heroku, we need 

1. HEROKU_EMAIL=pallavi.kharbanda01@gmail.com
2. HEROKU_API_KEY=<>
3. HEROKU_APP_NAME=mlproject-deployment

Build Docker Image
```
docker build -t <image_name>:<tagname> .
```
< Note: Image name for docker must be lowercase

To list docker image
```
docker images
```
Run docker image

```
docker run -p 5000:5000 -e PORT=5000 f8c749e73678 (# Image_ID)
```

To check running container in docker
```
docker ps
```
To stop docker container
```
docker stop <container_id>
```





