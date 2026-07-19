# Code Review Prompts

Use these prompts when asking an AI agent to review code for quality, correctness, and maintainability.

---

## Thorough Code Review

```
Please review the following code thoroughly. For each issue you find, indicate:
1. The severity (critical / major / minor / suggestion)
2. The exact location (file and line number if possible)
3. A clear explanation of the problem
4. A concrete recommendation or fix

Also highlight anything that is done particularly well.

<code>
[PASTE CODE HERE]
</code>
```

---

## Security-Focused Review

```
Review the following code specifically for security vulnerabilities. Check for (but don't limit yourself to):
- Injection attacks (SQL injection, OS command injection, LDAP injection, XPath injection, NoSQL injection)
- Insecure deserialization
- Hard-coded secrets or credentials
- Improper authentication / authorization
- Sensitive data exposure
- Dependency vulnerabilities

For each finding, provide the severity (critical / high / medium / low), a description, and the recommended fix.

<code>
[PASTE CODE HERE]
</code>
```

---

## Performance Review

```
Analyze the following code for performance issues. Consider:
- Time and space complexity of algorithms
- Unnecessary re-computations or repeated database/API calls
- Memory leaks or excessive allocations
- Blocking operations that could be made asynchronous
- Missing indexes or inefficient queries

Rank findings by potential impact and suggest optimizations with example implementations where possible.

<code>
[PASTE CODE HERE]
</code>
```

---

## Readability & Maintainability Review

```
Review this code for readability and long-term maintainability. Evaluate:
- Naming clarity (variables, functions, classes)
- Function and class size / single-responsibility adherence
- Code duplication (DRY violations)
- Comment quality (missing, misleading, or outdated comments)
- Consistency with common conventions for [LANGUAGE/FRAMEWORK]

Provide specific, actionable suggestions to make the code easier to understand and maintain.

<code>
[PASTE CODE HERE]
</code>
```

---

## Pull Request Review Checklist

```
I'm about to merge the following diff. Act as a senior engineer and review it using this checklist:

- [ ] Logic correctness — does it do what it claims?
- [ ] Edge cases — are null/empty/boundary values handled?
- [ ] Error handling — are errors caught and surfaced appropriately?
- [ ] Tests — are there adequate tests for new behaviour?
- [ ] Breaking changes — could this break existing callers?
- [ ] Documentation — are public APIs/interfaces documented?

Highlight any checklist items that need attention, and provide specific feedback.

<diff>
[PASTE DIFF HERE]
</diff>
```
