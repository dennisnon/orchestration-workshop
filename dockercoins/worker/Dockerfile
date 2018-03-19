FROM python:3-slim-stretch
RUN pip install redis
RUN pip install requests
COPY worker.py /
CMD ["python", "worker.py"]
