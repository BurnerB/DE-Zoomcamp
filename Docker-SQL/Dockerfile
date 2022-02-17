# Base Image
FROM python:3.9

RUN apt-get install wget
RUN pip install pandas sqlalchemy psycopg2

# directory image will load into on running
WORKDIR /app
COPY ingest_data.py ingest_data.py

ENTRYPOINT [ "python","ingest_data.py" ]