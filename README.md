     _  _____ _   _ ____   _____     _____ _   _ 
    / \|_   _| | | / ___| / _ \ \   / /_ _| \ | |
   / _ \ | | | |_| \___ \| | | \ \ / / | ||  \| |
  / ___ \| | |  _  |___) | |_| |\ V /  | || |\  |
 /_/   \_\_| |_| |_|____/ \___/  \_/  |___|_| \_|

Bookstore Program Code Flow:
   |__Struct book: Here we declared variables for book details.
   |
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
  		|	|__enter(): Here we have to parts in this function.
   		|	|	|
   		|	|	|__:Entering the book details
   		|	|	|
   		|	|	|__:Adding number of book entries
   		|	|--update_record(): For updating stock and price in record.
   		|	|	|
   		|	|	|__:Updating structure for changing book stock and price
   		|	|	|
   		|	|	|_____:Updating stock and Updating Price details
   		|	|	|
   		|	|	|________:Changing the file with updated stock and price.
   		|	|
   		|	|--update_pass(): For changing user password of user.
		|	|
   		|	|--Redirection function for redirecting to book store (services for customer).
		|	|
   		|	|--Exit.
   		|
   		|__:User Engine: Here we have services for interacting with the customer.
   			|--purchase(): A function where the User can purchase a book from the store.
			|	|	Here we have three steps to make the function interactive.
   			|	|
   			|	|__:Updating structure for dealing operation
   			|	|
   			|	|__:Accepting serching details for purchase
   			|	|
   			|	|__:Changing the file with new details of stock after purchase
			|	
   			|--complete_detail(): For checking all books detail.
			|	|		Here we have two steps for checking details
   			|	|
   			|	|__:Updating structure for printing operation
   			|	|
   			|	|__:Printing details of all books available in store in a tabular format.
			|
   			|--keyword(): For searching through keyword.
			|	|	Here we have two steps for keyword based book searching.
			|	|
   			|	|__:Updating structure for keyword operation
   			|	|
   			|	|__:Entering keyword to find words that matches the keyword with our book database and display it.
			|
   			|--others(): For all other operations. Here we have two functions for others.
			|	|	They are used for finding specific details of books in sub menu.
   			|	|
   			|	|__:Updating structure for all other operation
   			|	|
   			|	|____:Here we are giving 8 different operations:
  			|		|--a. Display All Books with Author Name 'Nark John'
   			|		|--b. Sort according to Price (Low to High)
   			|		|--c. Display not available Books
   			|		|--d. Display books whose name start with S
   			|		|--e. Display books of SChand Publisher
   			|		|--f. Display books of price between 100 to 500
   			|		|--g. Display all the books whose title is 10-20 characters
   			|		|--h. Exit Sub-menu
   			|--Exit.


We have created a book store with admin login function and comiled it all into Standalone Executable Format(.exe)
