FROM python:3.9

RUN pip install flask gunicorn python_jwt jwcrypto six

ADD ./app.py .

CMD gunicorn -w1 -b "0.0.0.0:80" app:app