from airflow import DAG
from airflow.operators.python_operator import PythonOperator
from datetime import datetime

def print_hello():
    print("Hello, World!")

dag = DAG('hello_world', description='Simple DAG that prints Hello World!',
          schedule_interval=None, start_date=datetime(2023, 10, 1), catchup=False)

hello_task = PythonOperator(
    task_id='print_hello_task',
    python_callable=print_hello,
    dag=dag,
)
