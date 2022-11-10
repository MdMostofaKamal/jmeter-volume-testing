# jmeter-volume-testing-with-jdbc-connection

 Here user information is read from a specific database and users are inserted.Volume testing is performed by increasing threads and rampup in Jmeter. Steps taken to build this project:
- JDBC connection is configured by connecting a specific Database where there is pre-existing datas
- JDBC driver class (com.mysql.jdbc.Driver) is configured
- mysql-connector-java is put in the lib folder of apache-jmeter
- Local-database is tested for read operation 100 users in 60s

![read operation test for 100 user in 60s](https://user-images.githubusercontent.com/47362218/201136383-2eb50a85-2bb4-499d-8bfe-aa8cacb8219c.PNG)

- Error 0.00%

- Local-database is tested for read operation 300 users in 60s

![read operation test for 300 user in 60s](https://user-images.githubusercontent.com/47362218/201136852-f8297a06-e37f-45a5-b50d-e3e1a61a031d.PNG)

- Error 49.67%

- Local-database is tested for insert operation 100 users in 60s

![insert operation  test for 100users in 60s](https://user-images.githubusercontent.com/47362218/201137449-10cfa7c1-74df-466d-96f1-992cbc555b51.PNG)

- Error 0.00%

- Local-database is tested for insert operation 300 users in 60s

![insert operation test for 300users in 60s](https://user-images.githubusercontent.com/47362218/201137633-334d57e0-edb3-4b61-973c-ca82f08b4792.PNG)

- Error 49.67%

- Local-database is tested for insert and read operation 167 users in 60s

![insert and read operation test for 167users for 60s](https://user-images.githubusercontent.com/47362218/201138061-5c7b5272-0fad-4339-a238-915cc8940aaf.PNG)

- Error 9.58%

- Local-database is tested for insert and read operation 167 users in 65s

![insert and read operation test for 167users in 65s](https://user-images.githubusercontent.com/47362218/201138450-8008c2f5-1be5-447d-bd01-177d294716e4.PNG)

- Error 2.40%

- Local-database is tested for insert and read operation 167 users in 68s

- Error 0.00%

 After increasing time and keeping same amount of users , the error rate is 0% for 68s and can be regarded as the lower bottleneck of the test
 
 - Just Clone this project and run it your own database


