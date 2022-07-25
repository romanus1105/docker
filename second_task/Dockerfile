FROM python:latest

COPY . .
RUN pip3 install --no-cache-dir --upgrade -r requirements.txt

EXPOSE 8000

WORKDIR .

CMD ["python3", "manage.py", "migrate"]
CMD ["python3", "manage.py", "migrate", "--run-syncdb"]
CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]