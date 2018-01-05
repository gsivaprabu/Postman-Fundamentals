#  Postman Fundamentals - 03 Postman Basics - 02 GETting Books

[http://localhost:3000/landing](http://localhost:3000/landing)

- http://localhost:3000/books enter in postman client means throws 403 Forbidden error()

- Add  in headers parameter
	G-TOKEN : ROM831ESV
- Now you can get the book details 200 success status.
- Time and size also.

- [http://localhost:3000/books/1] (http://localhost:3000/books/1) get the book id 1 details

- [http://localhost:3000/books/search](http://localhost:3000/books/search) parameter need to pass
	- title 'waste'
	- author 'john'
	- http://localhost:3000/books/search?title=waste&author=john
	- Check unchecked the parameters

- Possible to save and download the response