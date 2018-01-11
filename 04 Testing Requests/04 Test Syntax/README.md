# Postman Fundamentals - 04 Testing Requests - 04 Test Syntax

- More test scripts

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```

- pm => postman name-space object
- test => test function
	- Two parameters
		- Name
		- Function to be executed the test
- response => response object
- pm object have several properties

- We can use environment variables
	- info
	- globals
	- environment
	- assertions (have.)

- More about [https://www.getpostman.com/docs/]	(https://www.getpostman.com/docs/)