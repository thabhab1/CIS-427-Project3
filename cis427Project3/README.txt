https://github.com/thabhab1/CIS-427-Project3
-----------
Team Members

- Thabet Habhab
- Ali Hazime
- Fatima Kourani
- Hassan Bazzi
-----------

All commands that have been asked for have been implemented, from the Login to the Shutdown and all operations in between.
To build and run my program, simply start the server and then the client (I used Apache Netbeans) the login using LOGIN username password
Commands must be capitalized and there can be no extra spaces such as LOGIN john john22 (one space right after john22) and error handling has been implemented. I have tested all functionality of the program and have not found any bugs.

Client output from my program:


Please login, type (LOGIN username password)
LOGIN
Server: 300 Invalid Command. Please input a valid command (LOGIN, SOLVE, LIST, SHUTDOWN, LOGOUT)
L
Server: 300 Invalid Command. Please input a valid command (LOGIN, SOLVE, LIST, SHUTDOWN, LOGOUT)
LOGIN banana
Server: 300 Invalid Command. Please input a valid command (LOGIN, SOLVE, LIST, SHUTDOWN, LOGOUT)
LOGIN root 2
Server: Invalid login.
LOGIN root root22
Server: Logged in as root
LOGIN banana
Server: You are already logged in, please logout to login as another user
SOLVE
Server: Error: No shape found
SOlve
Server: 300 Invalid Command. Please input a valid command (LOGIN, SOLVE, LIST, SHUTDOWN, LOGOUT)
SOLVE -r
Server: Error: No sides found
SOLVE -r 2
Server: Sides 2.0: Rectangle's perimeter is 8.00 and area is 4.00
SOLVE -r 2 3
Server: Sides 2.0 3.0: Rectangle's perimeter is 10.00 and area is 6.00
SOLVE -r 2 3 4
Server: Error: Invalid number(s)
SOLVE -c
Server: Error: Radius not found
SOLVE -c 3
Server: Radius is 3.0: Circle's circumference is 18.85 and area is 28.27
SOLVE -c 3 4
Server: Error: Invalid radius
SOLVE -c -r
Server: Error: Invalid number
SOLVE -c a 
Server: Error: Invalid radius
LIST
Server: 
root
	Radius is 3.0: Circle's circumference is 18.85 and area is 28.27
	Error: No shape found
	Error: No sides found
	Sides 2.0: Rectangle's perimeter is 8.00 and area is 4.00
	Sides 2.0 3.0: Rectangle's perimeter is 10.00 and area is 6.00
	Error: Invalid number(s)
	Error: Radius not found
	Radius is 3.0: Circle's circumference is 18.85 and area is 28.27
	Error: Invalid radius
	Error: Invalid number
	Error: Invalid radius

LIST -alL
Server: Error: Please input a valid command
LIST -all professor do you want to play valheim or phasmophobia with me
Server: Error: Please input a valid command
LIST -all
Server: 
john 
	Sides 3.0: Rectangle's perimeter is 12.00 and area is 9.00
	Sides 3.0 3.0: Rectangle's perimeter is 12.00 and area is 9.00
	Error: Invalid number(s)
	Error: No sides found
	Error: Missing shape and number(s)
	Error: Radius not found
	Radius is 3.0: Circle's circumference is 18.85 and area is 28.27
	Error: Invalid radius
	Error: Missing shape and number(s)
qiang 
	No interactions yet
root 
	Radius is 3.0: Circle's circumference is 18.85 and area is 28.27
	Error: No shape found
	Error: No sides found
	Sides 2.0: Rectangle's perimeter is 8.00 and area is 4.00
	Sides 2.0 3.0: Rectangle's perimeter is 10.00 and area is 6.00
	Error: Invalid number(s)
	Error: Radius not found
	Radius is 3.0: Circle's circumference is 18.85 and area is 28.27
	Error: Invalid radius
	Error: Invalid number
	Error: Invalid radius
sally 
	No interactions yet
MESSAGE john hello
From root: hello
MESSAGE -alL hello
Client is offline
MESSAGE -all hello
You are not the root user
MESSAGE -all hello
(Johns client)
From root: hello
(Qiangs client)
From root: hello
MESSAGE john 
300 Invalid Command. Please input a valid command (LOGIN, SOLVE, LIST, MESSAGE, SHUTDOWN, LOGOUT)

LOGOUT
Server: 200 OK


If typing "SHUTDOWN"
SHUTDOWN
Server: 200 OK