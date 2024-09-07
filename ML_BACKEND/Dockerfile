FROM python:3.10

WORKDIR /backend

COPY ./requirements.txt /backend/requirements.txt

RUN pip install --no-cache-dir --upgrade -r /backend/requirements.txt

# 
COPY ./app.py /backend/api

# 
CMD ["uvicorn", "app:app", "--host", "0.0.0.0", "--port", "8000"]