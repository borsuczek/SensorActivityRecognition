# 
FROM python:3.12-slim-bullseye

# 
WORKDIR /code

# 
COPY ./requirements.txt /code/requirements.txt

# 
RUN pip install --no-cache-dir --upgrade -r /code/requirements.txt

# 
COPY ./src .

# 
CMD ["uvicorn", "main:app","--host", "0.0.0.0", "--port", "80"]
