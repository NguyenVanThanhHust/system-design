FROM python:3.9

WORKDIR /code

COPY ./requirements.txt /code/requirements.txt

# RUN pip install  --no-cache-dir --upgrade -r /code/requirements.txt
RUN pip install --trusted-host pypi.org --trusted-host files.pythonhosted.org -r /code/requirements.txt

COPY ./app /code/app

CMD ["python", "app/main.py"]
