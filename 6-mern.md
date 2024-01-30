# Javascript

1. Explain the difference between var, let, and const in JavaScript.
2. How do JavaScript closures work?
3. Can you explain the concept of hoisting in JavaScript?

4. What are JavaScript prototypes?
5. What are arrow functions, and how do they differ from regular functions?

6. What is event loop in JavaScript and how does it work?

7. call vs bind vs apply

8. Guess the output:

a) let, var, const

```js
function test() {
    var x = 2;
    let y = 3;
    if (true) {
        var x = 5;
        let y = 6;
    }
    console.log(x);
    console.log(y);
}

test();
```

b) Execution Flow, Promise, and Timeout

```js
console.log('Script start');

setTimeout(function() {
    console.log('setTimeout');
}, 0);

Promise.resolve()
    .then(function() {
        console.log('promise1');
    })
    .then(function() {
        console.log('promise2');
    });

console.log('Script end');

```

c) hoisting

```js
function test() {
    console.log(a);
    console.log(foo());

    var a = 1;
    function foo() {
        return 2;
    }
}

test();

```

d)  Closure

```js
function test() {
    var arr = [];
    for (var i = 0; i < 3; i++) {
        arr.push(function() { console.log(i) });
    }
    return arr;
}

var output = test();
output[0]();
output[1]();  
output[2]();  
```

# Nodejs

1. What is Node.js and how is it different from traditional web servers?
2. How does Node.js handle child threads?

3. How does Node.js handle file operations, and what are the differences between synchronous and asynchronous file operations?
4. How can you monitor and improve the performance of a Node.js application?
5. What are streams in Node.js?
6. How do you ensure that your Node.js application scales well?


# Expressjs

1. What is the role of middleware in Express.js?
2. How do you serve static files in Express.js?
3. What is the purpose of app.use() in Express.js?
4. How do you manage sessions in Express.js?
5. API validation in express?

# Mongodb

1. Explain the difference between SQL and NoSQL databases, specifically MongoDB.
2. What is a document in MongoDB?
3. Describe what a collection in MongoDB is.
4. How does MongoDB handle relationships between data?
5. How can you achieve transaction-like functionality in MongoDB?

6. Can you explain the use of projection in MongoDB queries?
7. What is upsert in MongoDB?
6. Explain the $lookup operation in MongoDB.
8. How do you handle pagination in MongoDB queries?
9. $push, $each, modifier
10. $where Operator

