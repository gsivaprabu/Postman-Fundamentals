# Postman Fundamentals - 04 Testing Requests - 05 Basic Tests

- Check the count of the book

```javascript
pm.test("Status code is 200", function() {
    pm.response.to.have.status(200);
});

pm.test("Status code name has string", function() {
    pm.response.to.have.status("OK");
});

pm.test("Return 5 books", function() {
    const books = pm.response.json();
    pm.expect(books.length).to.eql(15);
});

const titleIsDefined = (book) => {
    return book.title !== undefined;
}

pm.test("All books have title", function() {
    const books = pm.response.json();
    pm.expect(books.every(titleIsDefined)).to.be.true;
});
```