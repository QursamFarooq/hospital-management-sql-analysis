# Hospital Management Data Analysis Using SQL

## Project Overview
This project uses MySQL to analyze a hospital management database, focusing on patient appointments, doctor activity, medication prescriptions, and hospital resources.

SQL queries are used to explore healthcare operations, identify patterns, compare performance across hospitals, and examine department room capacity.

The project demonstrates the practical application of relational database concepts, joins, aggregations, subqueries, Common Table Expressions (CTEs), window functions, and conditional logic to derive meaningful insights from structured data.

## Project Objectives

- Analyze hospital operations using a relational database.
- Examine patient appointment patterns and doctor activity.
- Investigate medication prescriptions and specialty utilization.
- Evaluate hospital resources, including departmental room capacity.
- Apply SQL techniques to extract meaningful insights from structured data.

## Key Questions Answered

- Which patients have more than three appointments or have returned for multiple visits?
- How do appointment volumes vary across hospitals and months?
- Which doctors have the highest appointment counts, and which have no appointments?
- Which patients have consulted doctors from multiple specialties?
- Which departments have the largest room capacity within each hospital?

## Dataset Description

The project uses a hospital management database containing related information about hospitals, departments, doctors, patients, appointments, medications, prescriptions, and rooms. The tables are connected through primary and foreign keys, enabling analysis across different aspects of hospital operations.

### Data Dictionary

| Table | Description |
|---|---|
| `hospitals` | Stores hospital information. |
| `departments` | Contains department details within hospitals. |
| `doctors` | Stores doctor information and medical specialties. |
| `patients` | Contains patient demographic and contact information. |
| `appointments` | Records patient appointments with doctors. |
| `medications` | Stores medication names and descriptions. |
| `prescriptions` | Links patients, doctors, and medications through prescription records. |
| `rooms` | Contains room numbers, department associations, and capacities. |

## Tools Used

- **MySQL:** Database querying and analysis.
- **MySQL Workbench:** SQL development, query execution, and result validation.

## SQL Analysis & Queries

The project applies a range of SQL concepts to analyze hospital data:

- **Filtering and Sorting:** `WHERE`, `ORDER BY`, and date functions.
- **Joins and Aggregations:** `JOIN`, `GROUP BY`, `HAVING`, and aggregate functions.
- **Subqueries and CTEs:** Simplifying complex queries and organizing intermediate results.
- **Window Functions:** Ranking doctors, identifying recent appointments, and analyzing patient visit patterns.
- **Conditional Logic:** `CASE` statements for patient age-group classification.
- **Distinct Counts:** Identifying unique specialties and frequently prescribed medications.

## Key Insights

The analysis shows:

- No patient had more than three appointments, but returning patients were common, with some coming back up to three times. The gap between visits varied widely, from as little as 3 days to about six months, which suggests a mix of quick follow-ups and routine care.
- Appointment volumes are low and uneven across hospitals, from 4 at Cedar Grove Community Hospital to 14 at Silver Oak Medical Center. Monthly counts stay between 1 and 4 per hospital, with no clear seasonal pattern.
- Daniel Wright (Northwind Regional Medical Center) handled the most appointments with 8, followed by James Lin (Riverside General Hospital) with 7, while the busiest doctor at most other hospitals handled between 3 and 6. No doctor had zero appointments, and the least busy doctors still had at least one.
- Out of 120 patients, 24 patients have seen doctors from more than one specialty.
- Pediatrics has the largest room capacity in four of the eight hospitals shown, followed by Radiology in two, and most hospitals’ top department has a total capacity of 6 rooms. Maplewood General Hospital is the exception, where Cardiology leads with a capacity of 4.

## Conclusion

This project used SQL to analyze hospital appointments, patient visits, doctors, prescriptions, and hospital resources. The analysis helped identify patterns in appointment volumes, patient activity, medication usage, and resource distribution. Overall, the project provided practical experience in querying healthcare data and extracting insights that can support better understanding of hospital operations.
