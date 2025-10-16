FROM python:3.8-slim-buster
LABEL maintainer="Emmanuel Edorh"
COPY techtrends /app
WORKDIR /app

RUN pip install -r /app/requirements.txt
RUN python init_db.py

CMD [ "python", "app.py" ]
EXPOSE 3111