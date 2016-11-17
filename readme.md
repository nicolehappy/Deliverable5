Deliverable 5 -- Security Testing

Yue Li (yul134)

Testing site: http://testphp.vulnweb.com

Vulnerability 1: Cross Site Scripting (Reflected) http://testphp.vulnweb.com/signup.php

	1. This vulnerability attacks integrity, which means the data of this site could be accessed by unauthorized users.
	2. It is modification
	3. It is active
	4. Due to this vulnerability, unauthorized access might occur.
	5. steps to exploit this vulnerability:
		(1). Go to sign up page.
		(2). Type "</li><script>alert(1);</script><li>" into username column.
		(4). Click "signup".
		Then we can see signup process will be successful.
	6. steps to fix this vulnerability: 

	