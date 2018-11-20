FROM python:3-alpine

COPY requirements.txt ./

RUN pip install -r requirements.txt
RUN mkdir logs

COPY . .

CMD ["python", "-u", "./front.py"]
