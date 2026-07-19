# Refactoring Prompts

Use these prompts to get AI assistance when refactoring code for improved clarity, structure, or performance.

---

## General Refactoring Request

```
Please refactor the following [LANGUAGE] code. My goals are:
- [GOAL 1, e.g. "improve readability"]
- [GOAL 2, e.g. "reduce duplication"]
- [GOAL 3, e.g. "follow [PATTERN/CONVENTION]"]

Constraints — do NOT change:
- The public API / function signatures (unless specified)
- behavior observable from the outside (all tests should still pass)

<code>
[PASTE CODE HERE]
</code>

After refactoring, briefly explain each significant change you made and why.
```

---

## Extract Reusable Functions / Modules

```
The following code contains logic that is repeated or could be extracted into reusable helpers. Please:
1. Identify the duplicated or extractable logic
2. Propose clear names for the new functions/modules
3. Show the refactored version with the helpers extracted

<code>
[PASTE CODE HERE]
</code>
```

---

## Apply a Design Pattern

```
I want to apply the [DESIGN PATTERN NAME] design pattern to the following code. Please:
1. Briefly explain why this pattern is appropriate here
2. Show the refactored code using the pattern
3. Point out any trade-offs or edge cases to be aware of

<code>
[PASTE CODE HERE]
</code>
```

---

## Simplify Complex Conditionals

```
The conditional logic in the following code is hard to follow. Please refactor it to be cleaner and easier to understand. Techniques you might use: early returns, guard clauses, extracted predicates, lookup tables, or polymorphism. Keep the behavior identical.

<code>
[PASTE CODE HERE]
</code>
```

---

## Modernize Legacy Code

```
This code was written for an older version of [LANGUAGE/FRAMEWORK]. Please update it to use modern idioms and best practices available in [CURRENT VERSION], while keeping the same external behavior.

Highlight what you changed and why the new approach is preferred.

<code>
[PASTE CODE HERE]
</code>
```

---

## Improve Error Handling

```
The error handling in this code is inconsistent or incomplete. Please refactor it to:
- Handle all foreseeable failure modes explicitly
- Use consistent error-handling patterns (exceptions vs error codes vs Result types — match the style already used in this codebase)
- Provide meaningful error messages that help diagnose problems
- Avoid swallowing errors silently

<code>
[PASTE CODE HERE]
</code>
```
