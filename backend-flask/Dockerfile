FROM python:3.10-slim-buster

#Inside Container - Make a new folder called backend-flask inside container
WORKDIR /backend-flask

#Outside Container --> Inside Container - This contains the libraries you want to install inside container to run the app
COPY requirements.txt requirements.txt

#Inside container - installs python libraries used for this app
RUN pip3 install -r requirements.txt

# . means everything in the current directory
# first . represents everything in backend-flask outside container. Second . represents everything in backend-flask inside container
COPY . .

#Set environemnt variables inside the container and will remain set when the container is running
ENV FLASK_ENV=development


EXPOSE ${PORT}
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]