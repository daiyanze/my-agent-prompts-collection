# Debugging Prompts

Use these prompts to guide an AI agent in systematically diagnosing and fixing bugs.

---

## Systematic Bug Investigation

```
I have a bug in my [LANGUAGE] code. Help me debug it systematically.

**Symptoms:** [DESCRIBE WHAT IS HAPPENING]
**Expected behaviour:** [DESCRIBE WHAT SHOULD HAPPEN]
**Steps to reproduce:** [LIST STEPS]

Here is the relevant code:

<code>
[PASTE CODE HERE]
</code>

And here is the error output / stack trace:

<error>
[PASTE ERROR HERE]
</error>

Please:
1. Identify the most likely root cause(s)
2. Explain why the bug occurs
3. Suggest a fix with example code
4. Recommend any defensive changes to prevent similar bugs in the future
```

---

## Explain an Error Message

```
I received this error and I don't fully understand it:

<error>
[PASTE ERROR MESSAGE / STACK TRACE HERE]
</error>

Context — the code being executed:

<code>
[PASTE CODE HERE]
</code>

Please:
1. Explain what the error means in plain language
2. Point to the exact location in the code that causes it
3. Provide a corrected version of the relevant code snippet
```

---

## Rubber Duck Debugging

```
I'm trying to debug a problem and want to think through it out loud. Please act as a rubber duck — ask me clarifying questions one at a time to help me reason through the issue myself. Only offer suggestions after I've had a chance to work through the logic. Don't give away the answer too quickly.

Here's what I'm dealing with: [DESCRIBE THE PROBLEM]
```

---

## Trace Execution Step by Step

```
Please trace through the execution of the following code step by step, showing the value of all relevant variables at each significant point. Assume the following inputs:

<inputs>
[DESCRIBE INPUTS]
</inputs>

<code>
[PASTE CODE HERE]
</code>

At the end, state the final output and whether it matches the expected result of [EXPECTED OUTPUT].
```

---

## Flaky Test Investigation

```
I have a test that passes sometimes and fails other times (a "flaky" test). Help me identify why.

**Test name / description:** [TEST NAME]
**Failure rate (approximate):** [e.g. "fails ~20% of the time"]
**Environment:** [CI system, OS, language version, etc.]

<test_code>
[PASTE TEST CODE HERE]
</test_code>

<production_code>
[PASTE RELEVANT PRODUCTION CODE HERE]
</production_code>

Common causes to consider: race conditions, time/date dependencies, random data, shared global state, network/filesystem side effects. Please identify the likely cause and suggest a fix.
```
