# System Database Administration

## Purpose

The System Database (System DB) is used for central administration of the SAP HANA system and management of tenant databases.

## Key Responsibilities

- Create Tenant Databases
- Start and Stop Tenant Databases
- Monitor System Landscape
- Manage System-Level Users
- Configure System Settings
- Perform System-Wide Administration

## Administration Activities

### Check Tenant Databases

1. Connect to System DB using HANA Studio.
2. Navigate to Landscape tab.
3. Review available tenant databases.

### Start Tenant Database

1. Connect to System DB.
2. Select Tenant Database.
3. Right-click and choose Start.

### Stop Tenant Database

1. Connect to System DB.
2. Select Tenant Database.
3. Right-click and choose Stop.

### Create Tenant Database

1. Connect to System DB.
2. Open SQL Console.
3. Execute database creation command.
4. Verify tenant status.

## Monitoring Activities

- Monitor Database Status
- Check Active Services
- Review Alerts
- Monitor Resource Usage
- Verify Database Connectivity

## Common Issues

### Unable to Connect to Tenant DB

Cause:
- Tenant database stopped
- Network issue
- Incorrect port

Resolution:
- Verify tenant database status
- Start database if required
- Check connectivity

### Tenant Database Not Visible

Cause:
- Incorrect system connection
- User authorization issue

Resolution:
- Connect to System DB
- Verify privileges

## Interview Question

### What is the role of System DB in SAP HANA?

Answer:
System DB is responsible for overall SAP HANA administration. It manages tenant databases, system configurations, monitoring, security settings, and system-wide operations.

## Related Topics

- MDC Architecture
- Tenant Database Administration
- HANA Services
- Backup and Recovery

## Result

System DB provides centralized administration and control of the SAP HANA landscape.
