# AHA!

**Who Needs an LLM to Program an LLM?**
A rank-one weight edit built from a model's own matched pairs and a linear
program, with no language model anywhere in the loop.

Read it: <https://haithamb.github.io/aha/>

By Ahmed Khamis, Rasul Tutunov and Haitham Bou Ammar.
Published 15 November 2026. Models: Qwen3.5-0.8B and 2B, thinking enabled.

## What this repository holds

`index.html` — the post itself, self-contained apart from its web fonts. No
build step, no dependencies. Open it locally, or let GitHub Pages serve it.

`aha_before_after.mp4` and `aha_before_after.gif` — the clip at the head of the
post: one GSM8K question answered twice, by the model as released and by the
same checkpoint with 16,241 weights changed. The post carries its own copy
inline, so these two are here only for reuse elsewhere.

## Credit

This post stands on work that was done first, and done in the open:

- **Rikiya Takehi, Jayden Teoh, Alex Zhang and Omar Khattab**, who released
  their agent's complete logs. Every claim made here about that agent is
  checkable only because they did.
- **Nathan Barry**, who rebuilt the edit from those logs and showed it is
  exactly rank one, ΔW = u v⊤; who timed the agent and found where its ten
  hours actually went; who offered an LLM-free direction that gets most of the
  way; and whose linear program replaced the slowest part of the search. His
  detector is used here unchanged.

Nothing here is offered as a correction to either. The question is a narrower
one: how much of the result survives when the language model is taken out of
the loop, and the fine-tuning budget with it.
