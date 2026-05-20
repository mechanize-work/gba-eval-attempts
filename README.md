# GBA Eval — Final Run Attempts

The nine emulator codebases produced by frontier AI coding agents in
the [GBA Eval](https://gbaeval.com) May 2026 leaderboard. Each agent
had 24 hours to write a complete software Game Boy Advance emulator
with WebAssembly support from scratch.

Each subdirectory under `models/` is a git submodule pointing at that
agent's standalone repo, pinned at the final checkpoint commit. Inside
each submodule, `git log` shows the sequence of autosave checkpoints
the agent committed across the 24 hours.

## The lineup

| Model              | Harness            | Repo                                                                                                  |
|--------------------|--------------------|-------------------------------------------------------------------------------------------------------|
| Claude Opus 4.7    | Claude Agent SDK   | [gba-eval-attempt-claude-opus](https://github.com/mechanize-work/gba-eval-attempt-claude-opus)         |
| Claude Opus 4.6    | Claude Agent SDK   | [gba-eval-attempt-claude-opus-4-6](https://github.com/mechanize-work/gba-eval-attempt-claude-opus-4-6) |
| Claude Sonnet 4.6  | Claude Agent SDK   | [gba-eval-attempt-claude-sonnet](https://github.com/mechanize-work/gba-eval-attempt-claude-sonnet)     |
| Gemini 3.1 Pro     | Gemini CLI         | [gba-eval-attempt-gemini-pro](https://github.com/mechanize-work/gba-eval-attempt-gemini-pro)           |
| Gemini 3.5 Flash   | goose (OpenRouter) | [gba-eval-attempt-gemini-3-5-flash](https://github.com/mechanize-work/gba-eval-attempt-gemini-3-5-flash) |
| GPT-5.4            | Codex CLI          | [gba-eval-attempt-gpt-5-4](https://github.com/mechanize-work/gba-eval-attempt-gpt-5-4)                 |
| GPT-5.5            | Codex CLI          | [gba-eval-attempt-gpt-5-5](https://github.com/mechanize-work/gba-eval-attempt-gpt-5-5)                 |
| Kimi K2.6          | goose (OpenRouter) | [gba-eval-attempt-kimi-k2-6](https://github.com/mechanize-work/gba-eval-attempt-kimi-k2-6)             |

## Cloning

```bash
git clone --recurse-submodules https://github.com/mechanize-work/gba-eval-attempts
```

Or, if already cloned without submodules:

```bash
git submodule update --init --recursive
```

To pull a single model's repo on its own:

```bash
git clone https://github.com/mechanize-work/gba-eval-attempt-gpt-5-5
```
