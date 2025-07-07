❌ Bad Code:

```javascript
function sum() {
  return a + b;
}
```

🔍 Issues:

- ❌ The function `sum` relies on global variables `a` and `b` without declaring or defining them within its scope. This
  makes the function unpredictable and prone to errors, as the values of `a` and `b` could change unexpectedly.
- ❌ The function doesn't accept any arguments, limiting its reusability and making it specific to the globally defined
  `a` and `b`.

✅ Recommended Fix:

```javascript
function sum(a, b) {
  return a + b;
}
```

💡 Improvements:

- ✔ The function `sum` now accepts `a` and `b` as parameters, making it a self-contained unit that doesn't rely on
  global variables.
- ✔ This makes the function reusable and predictable, as it will always return the sum of the two provided arguments.
- ✔ Using parameters improves the function's clarity and reduces the risk of unintended side effects.
