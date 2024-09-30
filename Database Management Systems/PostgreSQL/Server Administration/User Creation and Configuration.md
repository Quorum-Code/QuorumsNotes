#postgres 

# Roles and Users in Postgres

A User in Postgres is a Role which has the `LOGIN` attribute. A Role otherwise is a effectively the same as a Group.
## Role Attributes

Attributes can be given to Roles and provide certain permissions.
### Login
`LOGIN`
Enables database connection through the Role/Username.
### Super User
`SUPERUSER`
Bypasses all permission checks, except the right to log in. 
*Similar to `root` or `sudo`.*
### Database Creation
`CREATEDB`
Enables a user to be able to create databases.
### Role Creation
`CREATEROLE`
Enables a user to create, alter, and drop Roles.
### Initiating Replication
`REPLICATION`
Enables a role to be used for streaming replication.
### Password
`PASSWORD 'password'`
Enables password authentication to access the Role.
### Inheritance of Privileges
`INHERIT`
Enables a Role to inherit [[Role Privileges|Privileges]] from other Roles/Groups it is a part of.
*[[Explanation of Inherit Option]]*.
### Bypassing Row-Level Security
`BYPASSRLS`
Enables a Role to bypass every row-level security policy.
*[Talk on Row-Level Security in Postgres](https://www.youtube.com/watch?v=vZT1Qx2xUCo)*. [[Supabase Docs|Some more info on security]].
### Connection Limit

## Creating Users

## Creating a Basic User

Users in Postgres are Roles which have the `LOGIN` attribute. 

`CREATE ROLE [USERNAME] [ATTRIBUTE...];`

The commands below each achieve the same result.

`CREATE USER [USERNAME];`
`CREATE ROLE [USERNAME] LOGIN;`

# Privileges
# The Inherit Option

The Inherit option is a flag which enables the chaining of role or group privileges.

*[Source documentation.](https://www.postgresql.org/docs/17/role-membership.html#:~:text=Second%2C%20member%20roles%20that%20have%20been%20granted%20membership%20with%20the%20INHERIT%20option%20automatically%20have%20use%20of%20the%20privileges%20of%20those%20directly%20or%20indirectly%20a%20member%20of%2C%20though%20the%20chain%20stops%20at%20memberships%20lacking%20the%20inherit%20option.)*