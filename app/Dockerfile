# syntax=docker/dockerfile:1

FROM python:3.11.3-slim

COPY ./requirements.txt /app/requirements.txt

WORKDIR /app

RUN pip install --upgrade pip
RUN pip install --no-cache-dir -r requirements.txt

COPY . /app 

ENTRYPOINT [ "python" ]

CMD [ "hello.py"]
# CMD [ "python", "-m", "flask", "--app", "hello.py", "run" ]

EXPOSE 5000