# CookiesManager
A JavaScript library for creating, reading, modifying and deleting cookies with ease. With this library, you can easily manage your website's cookies and their attributes, such as name, value, and expiration date. The library provides a user-friendly interface for working with cookies, making it simple and straightforward to use.

[Click here to View the Library!](https://github.com/john-doe/my-repo/blob/main/example.txt)


## Features

- Create a cookie with a specified name, value, and number of days until expiration
- Create a cookie with infinite expiration time
- Read the value of a cookie by its name
- Delete a cookie by its name

## Usage

### Creating a Cookie

You can create a cookie by calling the `createCookie` function and passing in the name, value, and number of days until expiration:

```javascript
createCookie(name, value, days);
```
### Creating a Cookie with Infinite Expiration Time
You can create a cookie with infinite expiration time by calling the createCookieInfinite function and passing in the name, value, and either 0 or any falsy value for the days argument:
```javascript
createCookieInfinite("username", "John Doe", null); // or createCookieInfinite("username", "John Doe");
```

### Create Cookie with Expiration Date
To create a cookie with an expiration date, use the createCookie function. This function takes three arguments: name, value, and days.

The name argument is a string that represents the name of the cookie. The value argument is a string that represents the value of the cookie. The days argument is a number that represents the number of days until the cookie expires:
```javascript
createCookie("username", "John Doe", 7);
```

### Reading Cookies
To read a cookie, use the readCookie function. This function takes one argument: name. The name argument is a string that represents the name of the cookie you want to read.

The function returns the value of the cookie as a string, or null if the cookie does not exist.
```javascript
let username = readCookie("username");
console.log(username); // "John Doe"
```

### Deleting Cookies
To delete a cookie, use the deleteCookie function. This function takes one argument: name. The name argument is a string that represents the name of the cookie you want to delete.
```javascript
deleteCookie("username");
```
This code deletes the cookie named "username".

## Error Handling
You could add some error handling to the code to handle situations where the name argument is an empty string or undefined, and the value argument is undefined.

## Conclusion
This library provides a simple and easy-to-use solution for working with cookies in JavaScript. You can create cookies with an expiration date or with infinite time/days, read cookies, and delete cookies with just a few lines of code.


