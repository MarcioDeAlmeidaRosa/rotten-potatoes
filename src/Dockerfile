FROM python:3.8.12-buster

EXPOSE 5000

WORKDIR /app

COPY requirements.txt ./
COPY __pycache__/*.* __pycache__/

RUN pip install -r requirements.txt

COPY . .

ENTRYPOINT [ "python" ]

CMD [ "app.py" ]