# TWITTER DATA PIPELINE using APACHE AIRFLOW

### Introduction
* Twitter Data Pipeline using Apache Airflow is an end-to-end data engineering project that demonstrates how to extract data from Twitter, transform it, and automate the workflow using Apache Airflow. The pipeline fetches Twitter data using Python, organizes the ETL logic, and schedules it as a daily job using Airflow

### What This Project Does
* Extracts data from Twitter API: Uses Python (with libraries like Tweepy) to connect to Twitter and pull data programmatically. 

* Transforms data: Processes the raw tweet information into a structured format (e.g., using Pandas). 

* Orchestrates using Apache Airflow: Defines a workflow as a DAG (Directed Acyclic Graph) that runs the ETL process on a scheduled interval (e.g., daily). 

* Automates scheduling and monitoring: Airflow handles task dependencies, retries, and execution scheduling.

### Python Scripts

* twitter_etl.py: Contains the core ETL logic to connect to Twitter, extract data, transform it, and save the result. 

* twitter_dag.py: Defines the Airflow DAG that schedules and triggers the ETL function daily. 

* twitter_commands.sh: Helpful shell commands for setup and running the pipeline.

### Apache Airflow

* Airflow is used to orchestrate the ETL workflow, providing scheduling, logging, retries, and visualization of runs. 

* Workflows are defined as Python code (DAGs) for flexibility and maintainability.

### Workflow Summary

* Authenticate to Twitter API – Use your Twitter developer credentials to connect. 

* Extract data – Pull tweets or user info via Tweepy. 

* Transform with Python – Clean and structure the data using Pandas or custom logic. 

* Schedule with Airflow – Create a DAG that calls the ETL script on a recurring schedule (e.g., daily). 
  
  
