# Postman Fundamentals - 03 Postman Basics - 08 Import

- Creating a new book used POST method
- using [http://localhost:3000/ui](http://localhost:3000/ui)
- Adding the values for UI based

```curl
curl 'http://localhost:3000/books' -H 'Origin: http://localhost:3000' -H 'Accept-Encoding: gzip, deflate, br' -H 'Accept-Language: en,en-US;q=0.9,ta;q=0.8' -H 'User-Agent: Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36' -H 'Content-Type: application/json' -H 'Accept: */*' -H 'g-token: ROM831ESV' -H 'cache-control: no-cache' -H 'Referer: http://localhost:3000/ui' -H 'Connection: keep-alive' -H 'postman-token: 94e03697-36ba-33d0-bf88-eae6aeb4380e' --data-binary '{"title":"Wings of Fire","author":"Abdul Kalam","isbn":"06dbia4634","releaseDate":"01/01/2017"}' --compressed
```

- copy the curl details from browser
- Import have 4 options
	- Import File
	- Import Folder
	- Import From Link
	- Paste Raw Text

- We choose **Paste Raw Text**	
- Debugging API Calls easy
- Shopping cart is tedeaus to check, so we use CURL API import method