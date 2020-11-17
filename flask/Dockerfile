
# Pull Python3 base image
FROM python:3.8

# Set the working directory to /app
WORKDIR /code

# Transfer content from current dir to /app in container
ADD . /code

# Install python packages
RUN pip install -r requirements.txt

# Start uWSGI using config file
CMD ["uwsgi", "uwsgi.ini"]