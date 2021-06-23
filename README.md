# BOOKSTORE-ATHSOVIN

### Program Statement:
A book shop maintains the inventory of books that are being sold at the shop. The
list includes details such as author, title, price, publisher and stock position.
Whenever a customer wants a book, the sales person inputs the title and author and
the system searches the list and displays whether it is available or not. If it is not, an
appropriate message is displayed. If it is, then the system displays the book details
and requests for the number of copies required. If the requested copies are available,
the total cost of the required copies is displayed, otherwise the message “Sorry!
These many copies are not in stock” is displayed. Design a system using a class
called stock with suitable member functions and constructors.

|   `Specific task Group Member-1`   |
|:--------------------------------|
|   1. Display all the books whose author name is ‘Nark John’.   |
|   2. Display all the books along with their author, title, price and publisher sorted according to price lowest to highest.   |
|   3. Display all the books whose copies are not available in the stock.   |
|  `Specific task Group Member-2`  |
|   4. Display all the books whose names start with ‘S’.   |
|   5. Display all the details of the books whose publisher name is ‘SChand’.   |
|   6. Display all the books whose price is between 100 to 500.   |
|  `Specific task Group Member-3`  |
|   7. Display all the books whose title is between 10-20 characters.   |
|   8. Display all the books which are currently not available in the stock.   |

### Group Members:
1. [Souhardya Sarkar](https://github.com/s-vintagew)
2. [Bhavin Amesara](https://github.com/Bhavin-Amesara)
3. [Atharv Shirke](https://github.com/AtharvShirke9)

### Program Description:
* We made a program for the bookstore, in which we implemented security options of login to use the program. We have divided the program into two users. One is default “admin” and the second user we set. On the first run, we have to set up a username and password for a user, after setting up the user, will be asked to log in. As we log in, for the first time you will be logged into admin where we need to Input book details. After adding book details, We have to log out from **ADMIN** and have log in to **USER** for using the user section. From the user section, we can **PURCHASE** the book we want. We can see how many books are available in-store through the **DETAIL OF BOOKS** option. We can search for books, using any **KEYWORDS**. There is an option called **OTHERS** which has specified operation as per our problem statement. We have a **LOGOUT** option to switch between the users and **EXIT** for terminating the program. For the admin section, we must log out from the store and log in with admin credentials to get into the admin section. In the **ADMIN** section, we have options for adding a new book which we can use to enter book details. We can update the book stock and book price from the **UPDATE RECORD** option. We can change the password for the user if the user forgets the password from the **CHANGE PASSWORD** option. We have a **LOGOUT** option to switch between the users and **EXIT** for terminating the program and We compiled it all into _Standalone Executable Format(.exe)_


### Code Flow:
```
Start:
|
|__Struct book: Here we declared variables for book details.
|
|	
|__main(): Here we have two functions.
	|
	|__setpath(): This functions is used for locating and creating our files in directory [C:/Users/<Current Username>/Documents/Athsovin]
		|
	  	|__:set_password: For setting up user credentials for the first run of the program. 
	  	|
	  	|__:login_into_user: For logging into the user or admin.
		|
		|__engine(): Here we have two functions.
   		  	|
   		  	|__:Admin Engine: Here we have admin services.
			|	|
  		  	|	|__enter(): Here we have to parts in this function.
   	  		|	|	|__:Entering the book details
   	  		|	|	|____:Adding number of book entries
   		  	|	|
			|	|	
   		 	|	|__update_record(): For updating stock and price in record.
   		  	|	|	|__:Updating structure for changing book stock and price
   		  	|	|	|____:Updating stock and Updating Price details
   		  	| 	|	|______:Changing the file with updated stock and price.
   		  	|	|
   	  		|	|
   	  		|	|__update_pass(): For changing user password of user.
   		  	|	|
   	  		|	|
   		  	|	|__Logout.
   		  	|	|
   	  		|	|
   		  	|	|__Exit.
   		  	|
   	  		|
   		  	|__:User Engine: Here we have services for interacting with the customer.
				|
				|__purchase(): A function where the User can purchase a book from the store. Here we have three steps to make the function interactive.
   				|	|__:Updating structure for dealing operation
   				|	|____:Accepting serching details for purchase
   				|	|______:Changing the file with new details of stock after purchase
   		  		|
   	  			|	
   				|__complete_detail(): For checking all books detail. Here we have two steps for checking details
   				|	|__:Updating structure for printing operation
   				|	|____:Printing details of all books available in store in a tabular format.
   		  		|
   	  			|
   				|--keyword(): For searching through keyword. Here we have two steps for keyword based book searching.
   				|	|__:Updating structure for keyword operation
   				|	|__:Entering keyword to find words that matches the keyword with our book database and display it.
   				|
   				|
   				|__others(): For all other operations. Here we have two functions for others. They are used for finding specific details of books in sub menu.
   				|	|__:Updating structure for all other operation
   				|	|____:Here we are giving 8 different operations:
  				|			|__a. Display All Books with Author Name 'Nark John'
   				|			|__b. Sort according to Price (Low to High)
   				|			|__c. Display not available Books
   				|			|__d. Display books whose name start with S
   				|			|__e. Display books of SChand Publisher
   				|			|__f. Display books of price between 100 to 500
   				|			|__g. Display all the books whose title is 10-20 characters
   				|			|__h. Exit Sub-menu
   				|
   				|__Logout.
				|
   				|
   				|__Exit.

```
