version: "3"
services:
    sportsstore:
        build: .
        ports: - "5002:5002"
        environment: - ASPNETCORE_ENVIRONMENT=Production
        depends_on: - sqlserver
        sqlserver:
            image: "mcr.microsoft.com/mssql/server:2022-latest"
            environment:
                SA_PASSWORD: "123456a@"
                ACCEPT_EULA: "Y"