### Example ETL that loads data from S3 into Redshift using Apache Airflow

## Libraries
* datetime
* logging
* airflow

## Steps
* Create an Airflow connection via Postgres to your AWS cluster; call it 'redshift'.
* Create an Airflow connection with your AWS User credentials; call it 'aws_credentials'.
* Launch the Airflow web server to run the DAG.
