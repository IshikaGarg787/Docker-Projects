#stage1 Base image 994mb ~ 1.04gb
FROM python:3.11 AS builder

WORKDIR /app

COPY requirements.txt .

RUN pip install -r requirements.txt

#------
#stage2 base image 400mb
FROM python:3.11-slim 

WORKDIR /app

COPY --from=builder /usr/local/lib/python3.11/site-packages/ /usr/local/lib/python3.11/site-packages/

COPY . .

ENTRYPOINT ["python","run.py"]
