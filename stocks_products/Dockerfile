FROM python:3.9-alpine

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

WORKDIR /stocks_products
COPY . .

RUN pip install --upgrade pip
RUN pip install -r requirements.txt

RUN chmod +x entrypoint.sh
ENTRYPOINT ["sh", "entrypoint.sh"]