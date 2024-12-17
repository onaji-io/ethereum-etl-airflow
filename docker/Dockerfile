FROM python:3.8.18

COPY requirements_local.txt requirements_airflow.txt requirements_test.txt \ ./
RUN pip install --upgrade pip && \
    pip install \
    -r requirements_test.txt \
    -r requirements_local.txt \
    -r requirements_airflow.txt

ENTRYPOINT ["airflow"]
