# ProjectManagers_UsedCarRental_FullStack
FINAL ver.

How to set up the front end and back end.

1) In models.py , 
conn = mysql.connector.connect(
    host="localhost",
    user="root",
    password="1234",
    database="project_db",
    port=3305
)

Port # , host and user have to be changed to your device.
Using MySQLWorkbench , run the script to create all the tables in MySQL.
Execute boundary.py to run the server. 

Boundary.py -> Boundary
App.py -> Controller
listing.py,review.py,shortlist.py,user_account.py,user_profile.py -> Entity

test_auth.py is for testing.


Frontend HTML , .js communicates with Boundary.py 
Boundary.py communicates with frontend and app.py only
App.py communicates with Boundary.py and Models.py
Entity communicates with App.py only. ( Entity handles connections to MySQL And SQL Queries ) 
