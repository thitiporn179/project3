# project3 Building a Datawarehouse with BigQuery
# Getting Started
python -m venv ENV
source ENV/bin/activate
pip install -r requirements.txt

# Run ETL Script
python etl.py

# Set def main(dataset_id, table_id, file_path)
main(dataset_id="github", table_id="events", file_path="github_events.csv")

# Set Project ID
project_ID = ""XXX_PROJECT""

# Set Keyfile Path
keyfile = ""XXX_KEYFILE_PATH""

# Keyfile Path in GCP
IAM & Admin --> Service Accounts
Create Service Accounts : 
    Service accounts details: Service account name
    Grant account access to project: Role
    Grant user access to service account: Done
    Create private key type: JSON

# Load data to BigQuery
python etl.py

# Add Actor in ETL and show in BigQuery
Delete events
python etl.py
Create new events

# Query Data
SELECT type from 
