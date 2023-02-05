FROM python:3.9.16

WORKDIR /app

RUN apt-get update
RUN apt -y install python3-aiohttp
RUN pip install influxdb-client==1.36
RUN pip install pika

COPY /SERVICES/ANALITICA/funciones.py /app/funciones.py

CMD [ "python", "/app/funciones.py" ]