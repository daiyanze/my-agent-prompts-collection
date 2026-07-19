# General AI Agent Prompts

Use these meta-prompts to consistently get better, more reliable responses from any AI agent.

---

## Get a More Thorough Response

```
[YOUR QUESTION OR REQUEST]

Before you answer, take a deep breath and think step by step. Be thorough and consider edge cases, alternative viewpoints, and potential pitfalls. If you are unsure about anything, say so explicitly.
```

---

## Ask for Structured Output

```
[YOUR QUESTION OR REQUEST]

Please respond in a structured format:
1. **Summary** — a 1–2 sentence TL;DR
2. **Details** — the full explanation
3. **Key takeaways** — 3–5 bullet points
4. **Next steps** — what I should do with this information
```

---

## Request Multiple Options

```
[YOUR QUESTION OR REQUEST]

Please give me [NUMBER, e.g. "3"] distinct approaches or options. For each one:
- Describe the approach
- List the pros and cons
- State when it is the best choice

End with a recommendation based on [MY CONTEXT / CONSTRAINTS].
```

---

## Challenge Assumptions

```
[YOUR STATEMENT / PLAN / DESIGN]

Please critically evaluate this. Specifically:
1. What assumptions am I making that might not hold?
2. What could go wrong?
3. What am I missing or overlooking?
4. What would a devil's advocate say?

Be honest — I want genuine critical feedback, not reassurance.
```

---

## Explain Like I'm a Beginner

```
Please explain [TOPIC] as if I have no prior knowledge of it. Use simple language, everyday analogies, and concrete examples. Avoid acronyms and jargon unless you immediately explain them. Check your explanation at the end — would a complete newcomer understand it?
```

---

## Explain Like I'm an Expert

```
I have a deep background in [FIELD / TECHNOLOGY]. Please explain [TOPIC] at an expert level — skip the basics, use precise technical language, and focus on nuance, trade-offs, and non-obvious insights.
```

---

## Iterative Refinement

```
Here is my current draft / solution:

<draft>
[PASTE YOUR DRAFT HERE]
</draft>

Please suggest specific improvements. For each suggestion:
- Quote the part you're addressing
- Explain what's wrong or could be better
- Provide the improved version

Do not rewrite the whole thing — give me targeted, surgical feedback I can apply one piece at a time.
```

---

## Verify AI Output

```
You previously gave me this answer:

<previous_answer>
[PASTE AI'S PREVIOUS RESPONSE HERE]
</previous_answer>

Please review it critically:
1. Is every factual claim accurate?
2. Is the reasoning sound?
3. Did you miss anything important?
4. Are there any caveats or limitations you didn't mention?

Correct any errors and add any important omissions.
```

---

## Force a Concrete Recommendation

```
[YOUR QUESTION — e.g. "Should I use approach A or approach B?"]

I understand there are trade-offs. I'm asking for your best recommendation for my specific situation: [DESCRIBE CONTEXT].

Please give me a definitive answer and explain your reasoning. Do not hedge excessively or say "it depends" without telling me exactly what it depends on and what your recommendation is given those factors.
```

---

## Ask for Sources / Evidence

```
[YOUR QUESTION OR CLAIM TO VERIFY]

Please support your answer with:
- Specific evidence, data points, or examples
- References to well-known authoritative sources where applicable
- An explicit statement of your confidence level (high / medium / low) and why

Flag anything you are less certain about so I can verify it independently.
```
