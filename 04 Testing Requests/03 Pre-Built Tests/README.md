# Postman Fundamentals - 04 Testing Requests - 03 Pre-Built Tests

- 

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Status code name has string", function () {
    pm.response.to.have.status("OK");
});

```

- You can check the test cases at post man itself