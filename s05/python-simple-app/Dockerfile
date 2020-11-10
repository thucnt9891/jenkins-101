FROM python:3-alpine
WORKDIR /service
COPY requirements.txt .
RUN pip install -r requirements.txt
RUN apk --no-cache add curl
COPY . ./
EXPOSE 8080
ENTRYPOINT ["python3", "app.py"]
