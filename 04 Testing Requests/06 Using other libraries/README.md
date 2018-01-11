# Postman Fundamentals - 04 Testing Requests - 06 Using other libraries

- Additional libraries
	- supports lodash
	- path
	- assert
	- buffer
	- util
	- url
	- punycode
	- querystring
	- string_decoder
	- stream
	- timers
	- events

##### Without moment throws error()

```javascript
pm.test("Create date is equal to today",function(){
    const data = pm.response.json();
    
    pm.expect(moment(data.createdAt).format('MM/DD/YYYY')).to.eql(moment().format('MM/DD/YYYY'));
})
```	

##### Included moment library

```javascript
const moment = require('moment');

pm.test("Create date is equal to today",function(){
    const data = pm.response.json();
    
    pm.expect(moment(data.createdAt).format('MM/DD/YYYY')).to.eql(moment().format('MM/DD/YYYY'));
})
```

##### Lodash Support

```javascript
const moment = require('moment');

pm.test("Create date is equal to today",function(){
    const data = _.result(pm,'response.json');
    pm.expect(moment(data.createdAt).format('MM/DD/YYYY')).to.eql(moment().format('MM/DD/YYYY'));
})
```	