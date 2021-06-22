# BOOKSTORE-ATHSOVIN
### Program Description:
* We made a program for bookstore, in which we implemented security options of login to use the program. We have divided the program into two user. One is default “admin” and second user we set. At first run we have to setup username and password for user, after setting up the user, will be asked to login. As we login for first time you will be logged into admin where we need to Input book details. After adding book details, we can directly move to bookstore using Redirect option. As we move to Bookstore, we now have access to normal user, and we can’t revert to admin. From user section we can ***PURCHASE*** the book we want. We can see how many books are available in store through ***DETAIL OF BOOKS*** option. We can search for books using any ***KEYWORDS***. There's also option called ***OTHERS*** which has specified operation as per our problem statement. and ***EXIT***. Now for admin section we must exit the store and login with admin credentials to get into admin section. In ***admin*** we have options for adding new book which we can use to enter book details. We can update the book stock and book price from ***UPDATE RECORD*** option. We can change password for user if user forgets password from ***CHANGE PASSWORD*** option. We have one special option to directly move to BOOKSTORE(which we called user section) through ***REDIRECTION*** option and Last is ***EXIT***. and We comiled it all into Standalone Executable Format(.exe)

### Program Code Flow:
```
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
   		  	|	|__Redirection function for redirecting to book store (services for customer).
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
   				|__Exit.

```
