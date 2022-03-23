# Sparkify Cassandra Database

This database was created as a means to give fast writes and reads to the Sparkify data

## Project structure

The project has been created with the following structure:

```bash
├── Project_1B_ Project_Template.ipynb
├── README.md
├── docker-compose.yaml
├── event_data
│   └── YYYY-MM-DD-events.csv
├── event_datafile_new.csv
└── requirements.txt
```

- Project_1B_ Project_Template.ipynb: Notebook with the corresponding tables and queries.
- event_data: Folder with the raw data in csv files.
- event_datafile_new.csv: Processed data (actual input to the database).
- docker-compose.yaml: Docker compose file for Cassandra Database.
- requirements.txt: requirements for python env.


## Docker

A docker compose file is provided to run a Postgres Database locally for developing purposes. 

```bash
docker-compose up
```

## Usage

Execute the Jupyter notebook to process the files, create the database and do the queries. The docker container with the Database needs to be up and running.

The python libraries cassandra-driver and pandas where used in most of the implementation.