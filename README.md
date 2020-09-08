# sql_not_manager
query_to_find_someone_not_managing

https://www.testdome.com/questions/sql/workers/39226?visibility=3&skillId=17

An employee is a manager if any other employee has their managerId set to this employee's id. That means John is a manager if at least one other employee has their managerId set to John's id.

TABLE employees
  id INTEGER NOT NULL PRIMARY KEY
  managerId INTEGER REFERENCES employees(id)
  name VARCHAR(30) NOT NULL

Write a query that selects the names of employees who are not managers.


