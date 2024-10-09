FROM python:3

# setting working directory inside the container
WORKDIR  /usr/src/app

# copy all lib in local to docker container
COPY requirements.txt ./

# install al package within thr requirements
RUN pip install --no-cache-dir --upgrade -r ./requirements.txt

# Docker listen at port 3001
EXPOSE 3001

# the command will be executed when the container starts
CMD ["python", "./src/server.py"]