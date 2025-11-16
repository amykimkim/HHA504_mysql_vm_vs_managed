
Region: us-central1 (Iowa)

Code would not run and gave error message:
"sqlalchemy.exc.OperationalError: (pymysql.err.OperationalError) (2003, "Can't connect to MySQL server on '34.59.233.219' (timed out)")"

Troubleshooting:
I tried to ping 34.59.233.219 on my terminal which was successful
Verified I configured to allow incoming connections on port 3306
Used public IP