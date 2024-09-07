# CommandBox Steps setting up a  CF Instance

if you are wanting to use MySQL 

> C:\drivers\mysql-connector-j-8.4.0.jar

1. Choose Web folder
> c:\example

2. in webroot folder
> install commadbox-cfconfig

3. Start new server in webroot folder port not required 
 
> server start port=8080 cfengine=adobe

4. To Set Password in webroot folder 

> cfconfig set adminPassword=myDevPassword to=example1


5. cfconfig import from=C:/coldfusion-config/datasources.json to=server

### FileName: 
>datasources.json
#### File Example
> {
  "dataSources": [
    {
      "name": "datasource_name",
      "driver": "com.mysql.cj.jdbc.Driver",
      "url": "jdbc:mysql://localhost:3306/database_name",
      "username": "username",
      "password": "password"
    }
  ]
}

6. server commands

- server help
- server list
- server stop
- server start
- server forget (delete)
- server clear (delete all)
- server log
