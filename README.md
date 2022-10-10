sudo apt-get update

################################
python installation
################################

sudo apt install python3-pip
sudo apt install python3-virtualenv
sudo apt install python3-pip

###############################
Virtual Environment
###############################

pip3 install venv airflow_workspace_name
cd airflow_workspace_name
source bin/activate

###############################
Export Home & Installation
###############################

export $AIRFLOW_HOME=~/airflow
pip3 install apache-airflow
airflow db init

###############################
Create username and password
###############################
airflow users create --username admin --firstname FIRST_NAME --lastname  LAST_NAME --role Admin --email admin@example.org
