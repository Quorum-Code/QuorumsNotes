#postgres #server-administration #users #roles #groups

# Roles

## Superuser

Command line prompt may look like `mydb=#` denoting you are accessing the database without access controls. Otherwise the prompt will look like `mydb=>`.
# Groups

Allows a database admin to group users and ease management of privileges. In practice Groups are user defined roles assigned to users.

## Creating a Group

`CREATE ROLE [GROUP_NAME];`
Creates a Role named `GROUP_NAME`.

## Assigning Group Membership

`GRANT [GROUP_NAME] TO [USERNAME];`
Grants `GROUP_NAME` Role's privileges to the user `USERNAME`.
## Removing Group Membership

`REVOKE [GROUP_NAME] FROM [USERNAME];`
Revokes `GROUP_NAME` Role's privileges from the user `USERNAME`.

## The Inherit Option

`{GRANT|REVOKE} [GROUP_NAME] {TO|FROM} [USERNAME] WITH INHERIT {TRUE|FALSE}, [SET {TRUE|FALSE}];`

Inherit should 
## Advanced Group Actions

More advanced Group actions are detailed in the [[Intro to Server Administration]].
# Next
[[User Creation and Configuration|Advanced Database Roles]]