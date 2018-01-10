# Postman Fundamentals - 03 Postman Basics - 10 Generating Code

- we can easily use code for inside applications
- Javascript code

```javascript
var settings = {
  "async": true,
  "crossDomain": true,
  "url": "http://localhost:3000/books",
  "method": "POST",
  "headers": {
    "Origin": "http://localhost:3000",
    "Accept-Encoding": "gzip, deflate, br",
    "Accept-Language": "en,en-US;q=0.9,ta;q=0.8",
    "User-Agent": "Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36",
    "Content-Type": "application/json",
    "Accept": "*/*",
    "g-token": "ROM831ESV",
    "Cache-Control": "no-cache",
    "Referer": "http://localhost:3000/ui",
    "Connection": "keep-alive",
    "Postman-Token": "33702942-75e2-0f8b-9215-17eb60a68f8a"
  },
  "processData": false,
  "data": "{\"title\":\"Wings of Fire\",\"author\":\"Abdul Kalam\",\"isbn\":\"06dbia4634\",\"releaseDate\":\"01/01/2017\"}"
}

$.ajax(settings).done(function (response) {
  console.log(response);
});
```