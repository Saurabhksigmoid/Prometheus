FROM python:slim

# This is to work in the directory.
WORKDIR /usr/local/app_info

# copy the requirement file to install the required packages. 
COPY ./app_info/requirements.txt .

# fire the run command to install the packages
RUN pip3 install -r requirements.txt

# copy the python code to run on container
COPY ./app_info/code.py .

# run the python command to execute the python code
CMD ["python" , "code.py"]