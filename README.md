#Deliverable 5 -- Security Testing

Yue Li (yul134)

Testing site: http://testphp.vulnweb.com

###Vulnerability 1: Cross Site Scripting (Reflected) http://testphp.vulnweb.com/signup.php

	1. This vulnerability attacks integrity, which means the data of this site could be modified by unauthorized users.
	2. It is modification attack
	3. It is active
	4. Due to this vulnerability, unauthorized access might occur.
	5. Steps to exploit this vulnerability:
		(1). Go to sign up page.
		(2). Type "</li><script>alert(1);</script><li>" into username column.
		(4). Click "signup".
		Then we can see signup process will be successful.
	6. Steps to fix this vulnerability:
Screenshots for this vulnerability:

1. signup page: <img src = "1_1.png">
2. sigup successfully: <img src = "1_2.png">
	
	
###Vulnerability 2: SQL Injection http://testphp.vulnweb.com/login.php

	1. This vulnerability attacks the confidentiality of the website, which means the data of this site could be modified by unauthorized users.
	2. It is interruption attack and modification attack
	3. It is active
	4. Business
	5. Steps to exploit this vulnerability:
		(1) Go to login page.
		(2) Type "test" as username.
		(3) Type "ZAP' OR '1'='1' -- " as password.
		(4) Click "login" button.
		Then we can see login is successful and user's profile is shown.
	6. Steps to fix this vulnerability:
Screenshots for this vulnerability:

1. login page: <img src = "2_1.png">
2. login successfully: <img src = "2_2.png">

###Vulnerability 3: SQL Injection -- MySQL http://testphp.vulnweb.com/signup.php
	1. This vulnerability attacks the confidentiality and integrity of the website, which means unauthorized users may read and write the data.
	2. It is interruption attack and modification attack and it is an active attack. 	
	3. It is active
	4. Business
	5. Steps to exploit this vulnerability:
		(1) Go to signup page.
		(2) Enter query "ZAP' UNION ALL select NULL -- " into username column.
		(3) Fill other columns.
		(4) Click "signup".
		Then the query will be executed and a message saying that the number of columns for the SELECT statement was incorrect.
	6. Steps to fix this vulnerability: 

