# [CookiesManager](https://github.com/Spookesites/CookiesManager/blob/main/cookiesManager.js)
A JavaScript library for creating, reading, modifying and deleting cookies with ease. With this library, you can easily manage your website's cookies and their attributes, such as name, value, and expiration date. The library provides a user-friendly interface for working with cookies, making it simple and straightforward to use.

[Click here to View the Library!](https://github.com/Spookesites/CookiesManager/blob/main/cookiesManager.js)

#### 🙏 Credits

This project was brought to life with passion by **Spook**. I am overflowing with gratitude for the friends who have supported me and encouraged me along the way.

Without their unwavering help and inspiration, this project would not have been possible. Thank you from the bottom of my heart to all my amazing friends. You are truly the best.

---

🎉 Congratulations on your project! 🎉


## Features

- Create a cookie with a specified name, value, and number of days until expiration
- Create a cookie with infinite expiration time
- Read the value of a cookie by its name
- Edit A Cookie Name And Value
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

### Editing a Cookie

These functions allows you to edit the name and value of a cookie to change it as arguments.
```javascript
// Example of using the editCookieValue function
let currentCookieName = "userInformation";
let currentCookieValue = readCookie(currentCookieName);
let newCookieValue = "updatedValue";
editCookieValue(currentCookieName, currentCookieValue, newCookieValue);
```
```javascript
// Example of using the editCookieName function
let currentCookieName = "userInformation";
let currentCookieValue = readCookie(currentCookieName);
let newCookieName = "userDetails";
editCookieName(currentCookieName, currentCookieValue, newCookieName);
```

Note: The "editCookieValue" and "editCookieName" functions should be implemented for the examples to work.

**Or if you want to do it the Classic way..**
```javascript
document.cookie = "cookie_name=new_cookie_value; expires=Thu, 18 Dec 2023 12:00:00 UTC; path=/";
```
In this example, the `cookie_name` is the name of the cookie you want to edit, and `new_cookie_value` is the new value you want to set for the cookie. The expires attribute sets the expiry date for the cookie, and the path attribute specifies the URL path for which the cookie is valid.

Note that in order for this to work, the new cookie must have the same name, path, and domain as the original cookie. Additionally, the new cookie must be set with the document.cookie property before the page is unloaded, as cookies are stored on the client-side and are not sent to the server unless a new request is made.

## Error Handling
You could add some error handling to the code to handle situations where the name argument is an empty string or undefined, and the value argument is undefined.

## Conclusion
This library provides a simple and easy-to-use solution for working with cookies in JavaScript. You can create cookies with an expiration date or with infinite time/days, read cookies, and delete cookies with just a few lines of code.



