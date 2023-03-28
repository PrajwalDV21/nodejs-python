FROM python:3.8

WORKDIR /app

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
RUN pip install --upgrade pip
RUN pip install psutil flask flask_cors

COPY . .
EXPOSE 5000
#CMD ["python3", "./app.py"]
CMD [ "python", "-m" , "flask", "run", "--host=0.0.0.0"]