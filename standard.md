## Code Standards

1. A set of rules or guidelines used when writing the code.
2. Generally dictates:
   Safety mandates to avoid introducing errors.
   Style mandates to increase maintainability.
   Security mandates to avoid vulnerabilities.
   Efficieny mandates to help performance.
3. Standards may be enforced through code reviews or may simply be "suggestions".

## Conventions

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
var a = 0;
var b = 5;
```

### Single Quotes
Unless you're writing JSON, please make sure you use single quotes.

**Incorrect**
```
var a = "something";
```

**Correct**
```
var a = 'something';
```