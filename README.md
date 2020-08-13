# Cloud-Research

# For Install PostgreSQL in Linux: <br /> 
sudo apt-get update <br /> 
sudo apt-get install postgresql postgresql-contrib <br /> 

# Check PostgreSQL status 
sudo systemctl status postgresql <br/> 
![](images/status.png)

# Connect to psql <br/> 
sudo su postgres <br/> 
psql <br/> 

another way to access: sudo -i -u postgres
![](images/access.png)

To access a Postgres prompt: psql  <br/> 
![](images/psql.png)

# For Exit: \q     
![](images/q.png)

# Create Database:
create database: create database db_name; <br/>
drop database: drop database db_name;  <br/>
show database: \l <br/>
Current Database and User: \c postgres;  <br/>
![](images/database.png)

# Create Table:
Example code: 
CREATE TABLE weather (
    city            varchar(80),
    temp_lo         int,           -- low temperature
    temp_hi         int,           -- high temperature
    prcp            real,          -- precipitation
    date            date
); <br/>
![](images/ntable.png)

# Inser data:
INSERT INTO weather VALUES ('San Francisco', 46, 50, 0.25, '1994-11-27'); <br/>
![](images/insert.png)

# View Data
Example code: SELECT * FROM weather; <br/>
![](images/view.png)

# Drop Table:
Example code: DROP TABLE weather; <br/>
![](images/drop.png)
