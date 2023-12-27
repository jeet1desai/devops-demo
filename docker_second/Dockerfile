FROM ubuntu:latest

WORKDIR /app

COPY . /app

RUN apt-get update && \
    apt-get install -y python3 python3-pip && \
    cd docker_second && \
    pip install -r requirements.txt

# ENTRYPOINT cannot be change
ENTRYPOINT ["python3"]
CMD ["manage.py", "runserver", "0.0.0.0:8000"]
