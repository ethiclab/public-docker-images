# ethiclab/sqlserver

    docker build -t ethiclab/sqlserver:1.0 .

# example

    docker run --env-file=$(pwd)/env -p 1433:1433 ethiclab/sqlserver:1.0

# env

    SA_PASSWORD=sUpeR5ecreT
    ACCEPT_EULA=Y
    MSSQL_PID=Express
