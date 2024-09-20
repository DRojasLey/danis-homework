# Guard Clauses

**What are Guard Clauses?**

In JavaScript, guard clauses are programming structures that check for invalid conditions at the beginning of a function. 

If a guard clause condition evaluates to `false`, the function immediately returns, preventing unnecessary execution.

**How to Use Them**

1. **Placement:** Typically, guard clauses are placed at the beginning of a function, before any other code.
2. **Conditions:** The conditions in guard clauses should be simple and easy to understand. They often check for null or undefined values, or if certain preconditions are met.
3. **Early Return:** If a guard clause condition evaluates to `false`, the function should immediately return with an appropriate value or throw an exception.

**When to Use Them**

- **Prevent Null or Undefined References:** Check for null or undefined values before accessing their properties or methods.
- **Validate Input:** Ensure that input parameters are valid and within expected ranges.
- **Handle Error Conditions:** Detect and handle potential errors early, preventing unexpected behavior.
- **Improve Readability:** By separating error handling from the main logic, guard clauses can make code more readable and easier to understand.

**Example:**

JavaScript

```js
function divide(dividend, divisor) {
    if (divisor === 0) throw new Error("Cannot divide by zero");
    
    return dividend / divisor;
}
```



In this example, the guard clause checks if the `divisor` is zero. If it is, an exception is thrown immediately, preventing a potential division by zero error.

#### Sources
https://pjmcdermott92.medium.com/writing-cleaner-javascript-with-guard-clauses-fe4bb8788425#:~:text=A%20guard%20clause%20is%20a,make%20functions%20shorter%20and%20cleaner.&text=error.

https://medium.com/@timothydan/javascript-guard-clauses-64b999e3240