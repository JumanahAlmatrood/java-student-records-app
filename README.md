# Java Login and Student Records App

A Java desktop application with a login window and separate pages for admins and users. It was built with Swing and connects to a Microsoft Access database through UCanAccess.

## Features

| Feature | Admin | User |
|---|---|---|
| Log in with a username and password | Yes | Yes |
| Save text to a `.txt` file | Yes | Yes |
| Search a file by student name or grade | Yes | Yes |
| Count how many students passed or failed | Yes | No |

A student passes with a grade of 10 or more.

## How it works

1. `Login.java` checks the username and password against the `DBlogin` table in `DBlogin.accdb`.
2. The user type in that record decides which page opens: `AdminPage` or `UserPage`.
3. `SearchPage` reads a file with one `name grade` pair on each line and shows the matching lines.
4. `StaticPage` reads the same format and shows the pass and fail counts.

## Tools

Java, Swing, JDBC, UCanAccess, Microsoft Access, Maven
