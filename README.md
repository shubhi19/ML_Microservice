[![CircleCI](https://circleci.com/gh/shubhi19/DevOps_Microservices.svg?style=svg)](https://circleci.com/gh/shubhi19/DevOps_Microservices)

## Project Overview

This project perationalizes a Machine Learning Microservice API. 

With a given pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. The data was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project operationalizes a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

The project uses [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. It performs the following operations :
* Tests project code using linting. 
* Dockerfile containerizes the application. 
* Creates a Kubernetes cluster.
* Deploy a container using Kubernetes and make a prediction.

The project has been tested with CircleCI and contains a test PASSED badge. The prediction outputs are showcased in folder `output_txt_files`.

## Project Components

### Dockerfile
Dockerfile creates a working directory and copies the source code to that directory. It installs the requirements listed in `requirements.txt` file and exposes port 80 from the container to the host. Lastly it runs the `app.py`. 

### Python Files
The project contains a single python file `app.py` which predicts housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, etc. 
#### Running Python Files 
python app.py 



