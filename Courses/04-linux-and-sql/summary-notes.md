# Linux and SQL - Summary Notes (Google Cybersecurity Professional Certificate)

## Module 1: Introduction to Linux

### What is Linux?
Linux is an open-source operating system that is widely used in servers, desktops, and embedded systems. It is known for its stability, security, and flexibility, making it a popular choice for cybersecurity professionals.

### Linux Distributions
- **Ubuntu**: User-friendly distribution for desktops and servers
- **CentOS**: Enterprise-grade distribution based on Red Hat Enterprise Linux
- **Debian**: Stable and reliable distribution for servers
- **Kali Linux**: Penetration testing and security auditing distribution

### Linux File System Hierarchy
- `/`: Root directory
- `/home`: User home directories
- `/etc`: Configuration files
- `/var`: Variable data files (logs, emails, databases)
- `/tmp`: Temporary files
- `/usr`: User programs and libraries
- `/bin`: Essential system commands
- `/sbin`: System administration commands

### Basic Linux Commands
- `ls`: List directory contents
- `cd`: Change directory
- `pwd`: Print working directory
- `cat`: Display file contents
- `mkdir`: Create directory
- `rmdir`: Remove directory
- `cp`: Copy file
- `mv`: Move file
- `rm`: Remove file

## Module 2: Linux File System

### File Permissions
- Linux uses a 3-digit octal system to represent permissions:
  - **0**: No permissions
  - **1**: Execute
  - **2**: Write
  - **3**: Write and execute
  - **4**: Read
  - **5**: Read and execute
  - **6**: Read and write
  - **7**: Read, write, and execute

- Permissions are divided into three categories:
  - **Owner**: Permissions for the file/directory owner
  - **Group**: Permissions for the file/directory group
  - **Other**: Permissions for all other users

### File Ownership
- `chown`: Change file owner
- `chgrp`: Change file group

### File Types
- **Regular files (-)**: Text files, binary files, etc.
- **Directories (d)**: Folders
- **Symbolic links (l)**: Links to other files/directories
- **Character devices (c)**: Input/output devices
- **Block devices (b)**: Storage devices
- **Pipes (p)**: Interprocess communication
- **Sockets (s)**: Network communication

## Module 3: Linux Commands and Shell Scripting

### Basic Linux Commands
- `grep`: Search for patterns in files
- `find`: Find files and directories
- `sort`: Sort file contents
- `uniq`: Remove duplicate lines
- `cut`: Extract specific fields from lines
- `paste`: Merge lines from files
- `head`: Display first lines of a file
- `tail`: Display last lines of a file

### Advanced Linux Commands
- `awk`: Text processing and data extraction
- `sed`: Stream editor for filtering and transforming text
- `xargs`: Build and execute command lines from standard input

### Shell Scripting Basics
- Shell scripts are text files containing a series of commands
- They are executed by the shell (bash, sh, csh, etc.)
- Shebang line: `#!/bin/bash`
- Variables: `name="value"`, `echo $name`
- Conditional statements: `if`, `elif`, `else`, `fi`
- Loops: `for`, `while`, `until`
- Functions: `function name() { commands }`

## Module 4: Linux User and Group Management

### User Accounts
- `useradd`: Create user account
- `usermod`: Modify user account
- `userdel`: Delete user account
- `passwd`: Change user password

### Group Management
- `groupadd`: Create group
- `groupmod`: Modify group
- `groupdel`: Delete group
- `gpasswd`: Add/remove users from groups

### Permissions and Access Control
- `chmod`: Change file permissions
- `chown`: Change file owner
- `chgrp`: Change file group
- `umask`: Set default permissions for new files

## Module 5: Introduction to SQL

### What is SQL?
SQL (Structured Query Language) is a programming language used to manage relational databases. It is used to query, insert, update, and delete data in databases.

### Relational Databases
- A relational database consists of tables that are related to each other
- Tables contain rows (records) and columns (fields)
- Relationships between tables are established using primary and foreign keys

### SQL Data Types
- **String types**: VARCHAR, CHAR, TEXT
- **Numeric types**: INT, BIGINT, DECIMAL, FLOAT
- **Date and time types**: DATE, TIME, DATETIME, TIMESTAMP
- **Boolean type**: BOOLEAN (or TINYINT(1))

### Basic SQL Statements
- `CREATE DATABASE`: Create a new database
- `USE`: Select a database to use
- `CREATE TABLE`: Create a new table
- `INSERT INTO`: Insert data into a table
- `SELECT`: Retrieve data from a table
- `UPDATE`: Update data in a table
- `DELETE FROM`: Delete data from a table
- `DROP TABLE`: Delete a table
- `DROP DATABASE`: Delete a database

## Module 6: SQL Queries

### SELECT Statement
- Basic syntax: `SELECT column1, column2 FROM table_name;`
- `*`: Select all columns
- `DISTINCT`: Remove duplicate rows

### WHERE Clause
- Filter rows based on conditions: `SELECT * FROM table_name WHERE condition;`
- Comparison operators: `=`, `<>`, `<`, `>`, `<=`, `>=`
- Logical operators: `AND`, `OR`, `NOT`
- Pattern matching: `LIKE` (e.g., `%`, `_`)
- Range: `BETWEEN`
- Membership: `IN`

### ORDER BY Clause
- Sort results: `SELECT * FROM table_name ORDER BY column_name [ASC|DESC];`

### LIMIT Clause
- Limit the number of results: `SELECT * FROM table_name LIMIT number;`

### Aggregate Functions
- `COUNT`: Count number of rows
- `SUM`: Calculate sum of values
- `AVG`: Calculate average of values
- `MIN`: Find minimum value
- `MAX`: Find maximum value

## Module 7: SQL Joins and Subqueries

### INNER JOIN
- Returns only the rows that match in both tables:
  ```sql
  SELECT t1.column1, t2.column2
  FROM table1 t1
  INNER JOIN table2 t2 ON t1.id = t2.id;
  ```

### LEFT JOIN (or LEFT OUTER JOIN)
- Returns all rows from the left table and matching rows from the right table:
  ```sql
  SELECT t1.column1, t2.column2
  FROM table1 t1
  LEFT JOIN table2 t2 ON t1.id = t2.id;
  ```

### RIGHT JOIN (or RIGHT OUTER JOIN)
- Returns all rows from the right table and matching rows from the left table:
  ```sql
  SELECT t1.column1, t2.column2
  FROM table1 t1
  RIGHT JOIN table2 t2 ON t1.id = t2.id;
  ```

### FULL OUTER JOIN
- Returns all rows from both tables:
  ```sql
  SELECT t1.column1, t2.column2
  FROM table1 t1
  FULL OUTER JOIN table2 t2 ON t1.id = t2.id;
  ```

### Subqueries
- A query within a query:
  ```sql
  SELECT column1
  FROM table1
  WHERE column2 IN (SELECT column2 FROM table2);
  ```

## Module 8: Database Security

### Database Authentication and Authorization
- **Authentication**: Verifying the identity of a user
- **Authorization**: Granting or revoking permissions to a user

### User Accounts and Permissions
- `CREATE USER`: Create a new user account
- `ALTER USER`: Modify a user account
- `DROP USER`: Delete a user account
- `GRANT`: Grant permissions to a user
- `REVOKE`: Revoke permissions from a user

### Database Encryption
- **Data at rest encryption**: Encrypting data stored on disk
- **Data in transit encryption**: Encrypting data sent over the network
- **Transparent Data Encryption (TDE)**: Encrypting entire databases

### Database Auditing and Monitoring
- **Audit logs**: Recording database activity
- **Monitor tools**: MySQL Enterprise Monitor, pgAdmin
- **Alerting**: Sending notifications for critical events
- **Compliance**: Ensuring compliance with regulations such as GDPR, HIPAA, and PCI DSS

## Key Takeaways

1. **Linux is essential for cybersecurity**: Linux is widely used in servers, firewalls, and other security devices
2. **File permissions are crucial**: Understanding Linux file permissions is important for securing systems
3. **SQL is used for data analysis**: SQL is used to query and analyze log data, which is essential for cybersecurity
4. **Database security is important**: Databases contain sensitive information and must be secured
5. **Shell scripting saves time**: Shell scripts can automate repetitive tasks, which is essential for security operations

## Best Practices Summary

- Use strong passwords for user accounts
- Implement least privilege access control
- Regularly update and patch systems
- Monitor system logs and database activity
- Use encryption to protect sensitive data
- Backup data regularly
- Train employees on security best practices
- Develop and test incident response plans

These summary notes are specifically aligned with the **Linux and SQL** course in the Google Cybersecurity Professional Certificate program, focusing on the skills and knowledge needed for entry-level Security Analyst roles.