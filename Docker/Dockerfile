FROM python:3.6-alpine

RUN pip install flask

COPY . /opt/

EXPOSE 8080

WORKDIR /opt

# entry point will be replaced by the command in the pod spec
ENTRYPOINT ["python", "app.py"]

#cmd will be overrriden by the arges in the pod spec
CMD ["--color", "red"]