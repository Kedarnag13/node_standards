## Code Standards

1. A set of rules or guidelines used when writing the code.
2. Generally dictates:
   Safety mandates to avoid introducing errors.
   Style mandates to increase maintainability.
   Security mandates to avoid vulnerabilities.
   Efficieny mandates to help performance.
3. Standards may be enforced through code reviews or may simply be "suggestions".

## Formatting

### Indentations
Two-spaces. Tabs are better, but they look bad on GitHub. Configure your editor appropriately.

### Trailing White spaces

**Incorrect**
```
var a = 0;//•••••
var b = 5;//••
```

**Correct**
```
var valueOfVaraibl1 = 0;
var valueOfVariable2 = 5;
```

### Single Quotes
Unless you're writing JSON, please make sure you use single quotes.

**Incorrect**
```
var name = "something";
```

**Correct**
```
var name = 'something';
```

### Opening braces always goes in the same line

**Incorrect**
```
if (condition)
{
  // statements
}
```

**Correct**
```
if (condition) {
  // statements
}
```

## Conventions

### LowerCamelCase for variables, function names
Also make sure the names are descriptive. Single character variables and uncommon abbreviations should generally be avoided.

**Incorrect**
```
var all_users = db.query("SELECT * FROM users");
```

**Correct**
```
var AllUsers = db.query("SELECT * FROM users");
```

### UpperCamelCase for class names

**Incorrect
```
function all_users() {

}
```

**Correct**
```
function AllUsers() {

}
```

### Use Ternary Operator
This is something new for me as well. As for Ruby, we're used to writing it in one line.

**Incorrect**
```
var name = ("something" === "something") ? "They are the same" : "They are not the same"
```

**Correct**
```
var name = ("something" === "something")
  ? "They are the same"
  : "They are not the same";
```

### Write Small functions
Functions should be coherent. It should be in such a way that it is written to accomplish a goal. So, how small is too small? It depends on the context. How easy it would be read code. If the name is descriptive and it's use is intuitive, size is almost irrelevant.

### Method chaining
One method per line should be used when you want chain methods. Also, keep me mind indenting the methods so it's easier to say as they are part of the same chain.

**Incorrect**
```
Resource.where({key: 'value'})
.has('new_value')
.exec(function (err, resource) => {
  return something;
});
```

**Correct**
```
Resource.where({key: 'value'})
  .has('new_value')
  .exec(function (err, resource) => {
    return something;
  });
```