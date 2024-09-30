#sql #postgres #dbms

# Intro to PostgreSQL

## What is PostgreSQL

**PostgreSQL** or **Postgres** is an Object-Relational Database Management System (ORDBMS) based on POSTGRES initially developed at UC Berkeley. 

## Getting Started with PostgreSQL

Refer to [[Spinning Up a PostgreSQL Server]] for details on getting a server and client ready.

## Configuring Admins and New Users

Refer to [[Basics of Users]] for details on how to add and configure users. 

*This note and the notes it points to are based off of the official [PostgreSQL 17.0 Documentation](https://www.postgresql.org/docs/17/index.html).*

## Accessing the Database

You can connect to the database using the commands listed [[Spinning Up a PostgreSQL Server#Connecting to PostgreSQL Server|here]].

---
# Useful Commands

## List Databases
`\l`

## Describe Users

`\du`
Reveals users with their [[Basics of Users#Roles|roles]] and [[Basics of Users#Groups|groups]]. 

---
# Next
[[Intro to Advanced Features in PostgreSQL]]