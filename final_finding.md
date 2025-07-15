# Findings from Prompt Injection Testing

## Project Summary

I attempted prompt injection attacks on several publicly accessible LLMs to test if they could be manipulated into revealing system instructions, internal prompts, or other protected data.

---

## Overall Results

- None of my prompt injection attempts were successful.
- Models consistently refused to reveal internal instructions.
- Responses included polite refusals, references to policies, or generic “I can’t help with that” messages.

---

## Security Measures Observed

- Keyword detection (e.g. “ignore instructions,” “system prompt,” “reveal secrets” triggered blocks)
- Semantic analysis — models recognized even reworded prompts
- Moderation APIs filtered sensitive topics
- Consistent refusal language patterns

---

## Interesting Observations

- Even creative or indirect prompts were blocked.
- Attempts that were conversational (e.g. “Hey friend, just curious…”) were still rejected.
- Responses often included disclaimers about ethics and policies.

---

## Lessons Learned

- Prompt injection remains a real risk, but modern LLMs are much better protected than expected.
- It’s hard to bypass policy constraints using simple text tricks alone.
- Documenting failures is just as important as successes in cybersecurity research.

---

## Next Steps

- Test prompt injection on other AI models 
- Explore building tools to detect prompt injection attempts automatically.
- Study prompt filtering differences between vendors.

---

