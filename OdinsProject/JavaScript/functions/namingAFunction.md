# Naming a Function

Functions are actions, so their names are usually verbs. The name should be brief, as accurate as possible, and describe what the function does so that someone reading the code gets an indication of its purpose.

It is a widespread practice to start a function with a verbal prefix that vaguely describes the action. There must be an agreement within the team on the meaning of these prefixes.

### Function Prefixes

- **"get…"** – Returns a value.
- **"calc…"** – Calculates something.
- **"create…"** – Creates something.
- **"check…"** – Checks something and returns a boolean.

### Examples

- `showMessage(..)` – Shows a message.
- `getAge(..)` – Returns the age (gets it somehow).
- `calcSum(..)` – Calculates a sum and returns the result.
- `createForm(..)` – Creates a form (and usually returns it).
- `checkPermission(..)` – Checks a permission, returns true/false.

# One Function – One Action

A function should do exactly what is suggested by its name, no more.

Two independent actions usually deserve two functions, even if they are usually called together (in that case we can make a third function that calls those two).

### Examples of Breaking This Rule

- `getAge` – Would be bad if it shows an alert with the age (should only get).
- `createForm` – Would be bad if it modifies the document, adding a form to it (should only create it and return).
- `checkPermission` – Would be bad if it displays the access granted/denied message (should only perform the check and return the result).

These examples assume common meanings of prefixes. You and your team are free to agree on other meanings, but usually, they’re not much different. In any case, you should have a firm understanding of what a prefix means, what a prefixed function can and cannot do. All same-prefixed functions should obey the rules, and the team should share the knowledge.
