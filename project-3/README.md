# DecodeLabs Project 3 - The Data Warehouse

## Objective
Provision a scalable managed cloud database using AWS RDS and store intern information in a MySQL database.

## AWS Services Used
- Amazon RDS (MySQL)
- Amazon EC2 (temporary SQL client)

## Database Details
- RDS Instance: `intern-database`
- Database: `InternDatabase`
- Engine: MySQL
- AWS Region: `eu-north-1` (Stockholm)

## Table Created
The `Interns` table contains the following columns:

| Column | Data Type |
|---|---|
| Name | VARCHAR(100) |
| Role | VARCHAR(100) |
| Email | VARCHAR(150) |

## Sample Records

| Name | Role | Email |
|---|---|---|
| Rahul Sharma | Cloud Intern | rahul@example.com |
| Priya Singh | DevOps Intern | priya@example.com |
| Arjun Kumar | AWS Intern | arjun@example.com |
| Ananya Patel | Cloud Engineer Intern | ananya@example.com |

## Implementation Steps

1. Created an Amazon RDS MySQL database.
2. Created a temporary Amazon EC2 instance to act as a SQL client.
3. Connected the EC2 instance to the RDS database.
4. Created the `InternDatabase` database.
5. Created the `Interns` table.
6. Inserted four dummy intern records.
7. Verified the records using `SELECT * FROM Interns;`.
8. Disconnected and reconnected to verify that the data persisted.
9. Terminated the temporary EC2 instance after completing the project.

## Result

The AWS RDS MySQL database was successfully provisioned, the `Interns` table was created, and the sample records were successfully inserted and verified.

## Evidence

Screenshots in this folder provide evidence of:

- RDS database creation and availability
- Table creation
- Intern records inserted into the database
- Data persistence after reconnecting
- Temporary EC2 client termination
