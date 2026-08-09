# New Flask Repo

A minimal Flask app that tests connectivity to a MySQL container running in Docker.

## What it does

Hits the `/` route, attempts to connect to a MySQL database, and returns a success message if the connection works — or the error if it doesn't. A simple sanity check for a Flask + MySQL Docker setup.

## Requirements

- Python 3
- Flask
- mysql-connector-python
- A running MySQL container reachable at host `mysql`, with a database named `devops`

## Running Locally

\`\`\`bash
pip install flask mysql-connector-python
python app.py
\`\`\`

The app runs on `http://0.0.0.0:5000`.

## Running with Docker Compose

Make sure your MySQL service is named `mysql` and has a database called `devops` set up, then:

\`\`\`bash
docker-compose up
\`\`\`

Vis
