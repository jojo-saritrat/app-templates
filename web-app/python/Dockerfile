FROM python:3.13-alpine

WORKDIR /app

COPY . /app

RUN pip install -r requirements.txt

EXPOSE 8000

ENTRYPOINT ["python"]

CMD ["main.py"]