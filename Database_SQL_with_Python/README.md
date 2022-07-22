# Databases and SQL for Data Science with Python
- API used by popular SQL-based DBMS systems:

|*Application or Database*                | *SQL API*        |
|-----------------------------------------|------------------|
|MySQL                                    | MYSQL C API      |
|PostgreSQL                               | psycopg2         |
|IBM DB2                                  | ibm_db           |
|SQL Server                               | dblib API        |
|Database access for microsoft window OS  | ODBC             |
|Oracle                                   | OCI              |
|Java                                     | JDBC             |

### Writing code using DB-API
from dbmodule import connect<br>
#Create connection object:<br>
conn = connect('databasename', 'username', 'password')

#Create a cursor object:<br>
cursor = conn.cursor()

#Run queries:<br>
cursor.execute('select * from mytable;')<br>
results = cursor.fetchall()

#Free resources:<br>
cursor.close()
conn.close()