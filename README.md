### Example ETL that loads data from S3 into Redshift using Apache Airflow

## Libraries
* datetime
* logging
* airflow

## Steps
* Create a Redshift cluster following the below requirements.
* Create an Airflow connection via Postgres to your AWS cluster; call it 'redshift'.
* Create an Airflow connection with your AWS User credentials; call it 'aws_credentials'.
* Launch the Airflow web server to run the DAG.


## Cluster requirements
Since data is hosted on Udacity's S3 @ us-west-2, cluster needs to follow the below criteria:
* Located in the us-west-2 region
* Publicly accessible (*open cluster --> actions --> modify to make publicly accessible*)
* The associated security group must allow the inbound traffic on the default port 5439 (*Cluster Parameters --> Network/Security settings --> VPC security group URL --> add an inbound rule for ALL TRAFIC with 0.0.0.0/0*)
