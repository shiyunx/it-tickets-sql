## IT Tickets Sql

This project analyses IT support tickets across departments to identify recurring issues and root causes using sql (sqlite) and python. It includes creating tables, inserting ticket data, and running SQL queries to calculate metrics such as ticket counts, average resolution times, and high-priority issues.

### Data Model

- **IT_Tickets**: Tickets with status, priority, resolution time, and created date

| TicketID | DepartmentID | RootCauseID | Status | Priority | Duration | Date       |
|----------|--------------|------------|--------|---------|---------|------------|
| 1        | 1            | 1          | Closed | High    | 5       | 2026-03-01 |
| 2        | 2            | 5          | Closed | Medium  | 8       | 2026-03-02 |
| 3        | 1            | 3          | Open   | Low     | 12      | 2026-03-03 |
| 4        | 5            | 1          | Closed | High    | 3       | 2026-03-04 |
| 5        | 4            | 4          | Open   | Medium  | 7       | 2026-03-05 |
| 6        | 2            | 2          | Closed | Low     | 4       | 2026-03-06 |
| 7        | 3            | 3          | Closed | High    | 6       | 2026-03-07 |
| 8        | 1            | 1          | Open   | High    | 9       | 2026-03-08 |
| 9        | 4            | 2          | Closed | Medium  | 2       | 2026-03-09 |
| 10       | 5            | 4          | Open   | Low     | 10      | 2026-03-10 |
| 11       | 5            | 2          | Closed | Low     | 4       | 2026-01-04 |
| 12       | 3            | 3          | Closed | High    | 6       | 2026-01-11 |
| 13       | 1            | 1          | Open   | Low     | 9       | 2026-03-01 |
| 14       | 4            | 5          | Closed | Medium  | 2       | 2026-01-03 |
| 15       | 5            | 4          | Open   | Low     | 10      | 2026-01-11 |

- **Departments**: Department names 

| DepartmentID | DepartmentName     |
|--------------|------------------|
| 1            | IT               |
| 2            | HR               |
| 3            | Finance          |
| 4            | Operations       |
| 5            | Customer Service |


- **RootCauses**: Types of IT issues 

| RootCauseID | RootCause         |
|-------------|-----------------|
| 1           | Configuration   |
| 2           | Software Failure|
| 3           | Network Issue   |
| 4           | Hardware Failure|
| 5           | Security        |