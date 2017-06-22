# Code 201, Day 13

Today in Code 201 we learned about persistence.  We've talked about 3 different methods of storing data:
* cookies
* localStorage
* sessionStorage

Of these three methods we worked on using localStorage for saving persistent data.  Of the three methods, it seems to be the most useful as it will maintain data between sessions even if the browser page is refreshed or shut down and restarted completely.

For localStorage we use four methods for altering data:
* setItem() to create or update a value in storage
* getItem() to retrieve and item in storage
* removeItem() to delete and item from storage
* clear() to remove all data from storage

Data is stored as key:value pairs, where both are required to be strings.  To store objects we first convert them to a string in JSON format using JavaScript methods JSON.stringify() to convert an object into JSON format and JSON.parse() to recover an object that has been stored in JSON format. Note: the object that is reconstructed is a new object, and not a copy of the reference to the original object.
