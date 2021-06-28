# car-brand-class
Deep learning project with data collection and some fun stuff

## Table of Content
  * [Demo](#demo)
  * [Overview](#overview)
  * [Installation](#installation)
  * [Deployement on Heroku](#deployement-on-heroku)
  * [Dataset](#dataset)
  * [Future scope of project](#future-scope)


## Demo
Deployment - Made the flask app just add the procfile and requirements.txt to deploy using heroku. [How to deploy](https://www.geeksforgeeks.org/deploy-python-flask-app-on-heroku/)

https://user-images.githubusercontent.com/51751926/123633904-68eb8b00-d837-11eb-85f6-4e788fdd9ffb.mp4

## Overview
This is a Flask web app which predicts the car name provided the car picture. 
<br/> Click on choose and upload an image to search <br/>
The model used was Resnet50 with fine tuing .Resnet50 and VGG models were used and Resnet came out to perform better

## Installation
The Code is written in Python 3.9.1. If you don't have Python installed you can find it [here](https://www.python.org/downloads/). <br/>
Make sure that pip is upgraded if not:
```bash
pip install --upgrade pip
```
- Cloning the repository :
     - 🦖 go to the folder in your device where you want to clone <br/>
     - 🦖 make sure that git is installed already if not click [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).
```bash
git clone https://github.com/amey16/Flight-fare-prediction.git
```
. If there is a slice error while running the code read the following points-
     . tensorflow.keras was depreciated to keras 
     . In order to run this particular model you need to have tenserflow.keras only
     . ```pip install tensorflow``` - specify version 2.0 if neccessary

## Deployement on Heroku
Login or signup in order to create virtual app. You can either connect your github profile or download ctl to manually deploy this project.

![image](https://user-images.githubusercontent.com/51751926/122658097-f61f4780-d186-11eb-8b74-2b37d9bbb4b9.png)
Click on the create app option once you reach this page
<br/>
Follow the instruction given on [Heroku Documentation](https://devcenter.heroku.com/articles/getting-started-with-python) to deploy a web app.


## Dataset

The dataset was made using web scraping of google images using the request and Beautiful_soup libraries <br/>
To know more about how i actually did web scraping [click here](https://github.com/amey16/Image-Web-Scraper) <br/>
<br/>
The dataset was collected for six cars namely mercedes , ferrari , bmw , lamborghini , tesla ,audi <br/>
How the images look after web scraped -<br/>
![image](https://user-images.githubusercontent.com/51751926/123635315-2b87fd00-d839-11eb-85f1-53f8c7bdd375.png)

<br/>
The testset was made manually by transfering some images from trainset

## Additional points
- Make sure that you have an empty uploads floder before you run the app
- If you want to install all libraries required for this project run these commands
    - pip install pipreqs
    - pipreqs "folder path"
- You can also try using VGG16 model it performs good on image datasets
## Future Scope

* Experiment aroud different architectures in transfer learning
* Improve the prediction accuracy then optimize Flask app.py and improve the UI 
