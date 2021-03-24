# AICamp CV Final Project - Face Recognition System

## Notice
   This is my project assignment from jiuzhang suanfa AI camp. please check the original code if needed (https://github.com/jiuzhangjiangzuo/AICamp-CV-Final_Project_Homework.git)
## Prework

Download the [model](https://drive.google.com/open?id=1EXPBSXwTaqrSC0OhUdXNmKSh9qJUQ55-) of facenet, and put all the files into `recognize/facenet_model`.

```
cp /path/to/unzip/dir/* recognize/facenet_model
```

## Run

### For Docker users

First, build the docker container.

```
docker build -t face .
```

Then, run the docker.

```
docker run -it -p 5000:5000 face python app.py
```

### For other users

First, install the python dependencies.

```
pip install -r requirements.txt
```

Then, run the webserver.

```
python app.py
```

## Implement

Please implement the empty parts in `detect/MtcnnDetector.py` and `recognize/facenet.py`