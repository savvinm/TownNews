FROM python:3.10.8
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
ENTRYPOINT  python3 manage.py migrate && \
            python3 manage.py runserver 0.0.0.0:8000