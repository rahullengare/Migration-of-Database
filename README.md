1. Create RDS Server
2. launch EC2 instance 
3. connect to ssh ec2 instance
4. mysql -u root -p (connect to local database)
5. create insta database
6. under insta database create user table with filed name, age, city
7. now exit to database
8. mysqldump -u root -p insta > insta.sql (all database copy into the insta.sql file)
9. this file cpoy in RDS server
10. mysql -h <RDS-end-point-here> -P 3306 -u admin -p dbname < insta.sql  (file copy ec2 server to RDS server) 
11. mysql -u <endpoint> -u admin -p (now checking) (log into the RDS server)
12. Enter Password to go to this RDS Server
13. Show Databases;
14. use insta;
15. show Tables;
16. select *from users;
17. now all data will be migrated…
