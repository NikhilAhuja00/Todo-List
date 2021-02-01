#Pull official base image
FROM python

#set Working Directory
WORKDIR /app/api
COPY . /app/api

#Install app dependencies
RUN pip install -r requirements.txt

#Add app

CMD ["python","manage.py","runserver","0.0.0.0:8000"]

#Expose the ports
EXPOSE 8000


