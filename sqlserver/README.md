# ethiclab/sqlserver

    docker build -t ethiclab/sqlserver:1.0 .

# example

    docker run --env-file=$(pwd)/env -p 1433:1433 ethiclab/sqlserver:1.0

# env

    SA_PASSWORD=sUpeR5ecreT
    ACCEPT_EULA=Y
    MSSQL_PID=Express

# hash

    1.0: digest: sha256:8f520f9631b7156b1e58b8c04cb44eb63e6b578bcd4d1da66d16b7dfd00e9b03 size: 3037
