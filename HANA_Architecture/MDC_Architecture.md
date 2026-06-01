# SAP HANA MDC Architecture

## Purpose

MDC (Multitenant Database Container) architecture enables multiple tenant databases to run within a single SAP HANA system.

## Components

### System Database

- Central administration database
- Manages tenant databases
- Maintains landscape configuration

### Tenant Database

- Stores application data
- Independent users and schemas
- Separate backups and monitoring

## Advantages

- Better resource utilization
- Simplified administration
- Enhanced isolation
- Easier database management

## Interview Question

What is the difference between System DB and Tenant DB?

Answer:
System DB is used for administration and managing tenant databases. Tenant DB contains business application data and is used by SAP applications.
