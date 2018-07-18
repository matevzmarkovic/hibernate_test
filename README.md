... following the Hibernate tutorial at [https://www.tutorialspoint.com/hibernate/hibernate_examples.htm].

# Postgres initialization

```
\connect test

CREATE TABLE EMPLOYEE (
   ID SERIAL NOT NULL,
   FIRST_NAME VARCHAR(20) DEFAULT NULL,
   LAST_NAME  VARCHAR(20) DEFAULT NULL,
   SALARY     INT  DEFAULT NULL,
   PRIMARY KEY (id)
);

CREATE SEQUENCE hibernate_sequence
INCREMENT 1
MINVALUE 1
MAXVALUE 9223372036854775807
START 1
CACHE 1;
```