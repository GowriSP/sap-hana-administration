# Tenant Database Administration

## Purpose

A Tenant Database (Tenant DB) stores SAP application data and is used by SAP systems such as S/4HANA for business operations.

## Responsibilities

- User Administration
- Role Management
- Schema Management
- Backup Monitoring
- Performance Monitoring
- Database Security

## Tenant DB Activities

### Connect to Tenant Database

1. Open SAP HANA Studio.
2. Add HANA System.
3. Select Tenant Database.
4. Enter Tenant DB credentials.
5. Connect successfully.

### User Management

Activities:

- Create Users
- Reset Passwords
- Lock Users
- Unlock Users
- Assign Roles

### Database Monitoring

Monitor:

- Memory Usage
- CPU Usage
- Active Sessions
- Alerts
- Expensive SQL Statements

### Backup Monitoring

Check:

- Data Backup Status
- Log Backup Status
- Backup Catalog
- Backup History

## Common Issues

### Unable to Add Tenant Database

Cause:

- Incorrect SQL Port
- Tenant Database Stopped
- Firewall Restrictions

Resolution:

- Verify Tenant DB Status
- Check SQL Port
- Validate Network Connectivity

### Authentication Failed

Cause:

- Incorrect Username or Password
- User Locked

Resolution:

- Reset Password
- Unlock User
- Verify User Authorization

### Tenant Database Not Responding

Cause:

- High Resource Utilization
- Service Failure

Resolution:

- Check HANA Services
- Review Alerts
- Analyze Resource Consumption

## Interview Scenario

### How do you connect to a Tenant Database?

Answer:

I use SAP HANA Studio or HANA Database Explorer. I select the Tenant Database, provide the SQL port, username, and password, then verify connectivity and database status before performing administrative activities.

### What happens if you connect to System DB instead of Tenant DB?

Answer:

System DB is used only for administrative tasks such as managing tenant databases. Business application data resides in the Tenant DB. If we connect to System DB instead of Tenant DB, application schemas and business data will not be accessible.

## Related Topics

- MDC Architecture
- System Database Administration
- HANA Services
- Backup and Recovery
- HDBSQL

## Result

Tenant Database Administration ensures secure, reliable, and efficient operation of SAP application databases in an SAP HANA environment.
