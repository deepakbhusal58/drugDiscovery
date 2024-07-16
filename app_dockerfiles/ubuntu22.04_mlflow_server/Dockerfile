FROM python:3.10.14-bookworm

RUN pip install mlflow==2.12.2

# EXPOSE 5000

CMD ["mlflow server --host 0.0.0.0 --port 5000 --backend-store-uri mysql://mlflow_user:mlflow@localhost:3306/db_mlflow --default-artifact-root var/lib/mlflow/mlruns"]