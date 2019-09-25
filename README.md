# 📦 Deploy a Keras Model with Flask

[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

Simple example of how to deploy a Keras image classification deep learning model using the Python micro web framework, Flask. 

![](keras-flask.gif)

__Technologies__

- Keras (Tensorflow)
- Flask
- Heroku

__Model__

For demonstration purposes this application loads the ResNet50 model from Keras applications. You can easily swap this out with the load_model function with your own trained and serialized model.

__Deployment__

This includes a Profile for Heroku to host and run the application. The Procfile just uses Green Unicorn as the server and prompts the flask application. You will need to link your GitHub account and create a Heroku account (free) to have this application in production.

__Development__

```sh
pip install -r requirements.txt

gunicorn app:app
```

