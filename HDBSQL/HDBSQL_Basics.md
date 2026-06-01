# HDBSQL Basics

## Purpose

HDBSQL is the command-line SQL interface used to connect and administer SAP HANA databases.

## Uses of HDBSQL

- Connect to SAP HANA Database
- Execute SQL Statements
- Create and Manage Users
- Monitor Database Objects
- Perform Administrative Tasks

## Basic Connection Syntax

```sql
hdbsql -n <hostname>:<port> -u <username> -p <password>
```

### Example

```sql
hdbsql -n localhost:30041 -u SYSTEM -p Password123
```

## Common Commands

### Check Current User

```sql
SELECT CURRENT_USER FROM DUMMY;
```

### Display All Users

```sql
SELECT USER_NAME FROM USERS;
```

### Create User

```sql
CREATE USER BASIS_USER PASSWORD Welcome@123;
```

### Reset Password

```sql
ALTER USER BASIS_USER PASSWORD NewPassword@123;
```

### Lock User

```sql
ALTER USER BASIS_USER DEACTIVATE USER NOW;
```

### Unlock User

```sql
ALTER USER BASIS_USER ACTIVATE USER NOW;
```

### Display Schemas

```sql
SELECT SCHEMA_NAME FROM SCHEMAS;
```

### Check Database Version

```sql
SELECT VERSION FROM SYS.M_DATABASE;
```

### Check Active Sessions

```sql
SELECT * FROM M_CONNECTIONS;
```

## Common Administrative Activities

### Verify Database Status

```sql
SELECT * FROM SYS.M_DATABASE;
```

### Monitor Memory Usage

```sql
SELECT * FROM M_HOST_RESOURCE_UTILIZATION;
```

### Check Services

```sql
SELECT * FROM M_SERVICES;
```

## Common Errors

### Authentication Failed

Cause:

- Invalid Username
- Incorrect Password
- User Locked

Resolution:

- Verify credentials
- Reset password
- Unlock user

### Connection Refused

Cause:

- Incorrect Hostname
- Incorrect Port
- Database Unavailable

Resolution:

- Verify hostname
- Check SQL port
- Confirm database status

## Interview Questions

### What is HDBSQL?

Answer:

HDBSQL is the SAP HANA command-line tool used to connect to HANA databases and execute SQL commands for administration, monitoring, and troubleshooting.

### Why do BASIS Administrators use HDBSQL?

Answer:

HDBSQL is used for user management, database monitoring, service checks, executing SQL queries, and performing administrative tasks when GUI tools are unavailable.

## Related Topics

- System Database Administration
- Tenant Database Administration
- HANA Services
- Backup and Recovery

## Result

HDBSQL provides a fast and efficient command-line interface for SAP HANA database administration and troubleshooting.
