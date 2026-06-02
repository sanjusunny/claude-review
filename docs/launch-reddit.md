# Reddit launch posts — claude-review

Repo: https://github.com/r3al1tymonster/claude-review
Skill install: `npx skills add r3al1tymonster/claude-review -g`
CLI install: `pipx install git+https://github.com/r3al1tymonster/claude-review`
Tagline: **Faster than HTML. Calmer than the terminal.**

## Posting plan

Post in this order, spaced out (not all same-day — every sub runs a qualitative
spam filter, and a fresh handle blasting 5 subs at once reads as spam). Reply to
comments on each before moving to the next.

1. **r/ClaudeCode** — highest intent, your core audience. Post first.
2. **r/SideProject** — self-promo explicitly welcome; easy early stars.
3. **r/commandline** — craft-forward; engage in comments, zero marketing tone.
4. **r/ChatGPTCoding** — use the **Project** flair.
5. **r/ClaudeAI** — biggest (~895k) but strictest quality bar; post last, value-first.

Runner-up: **r/Python** — great fit but gate to their weekly "Showcase" thread.

---

## 1. r/ClaudeCode

**Title:** I made a read-only "review pane" for Claude Code — latest response only, rendered, in a second terminal

Two-pane setup: I drive Claude Code on the left, and on the right a pinned pane
shows just the *latest* response as clean markdown, re-anchored to the top each
turn — never a scrolling log. `Tab` cycles response / plan / tasks. `f` freezes
the view while Claude keeps working.

Read-only, offline, sole dependency is `rich`. The idea: HTML reports are great
for deep reads, the raw stream is too fast to follow — this is the calm middle.
*Faster than HTML, calmer than the terminal.*

Install as a skill: `npx skills add r3al1tymonster/claude-review -g`
Repo: https://github.com/r3al1tymonster/claude-review

Feedback welcome.

---

## 2. r/SideProject

**Title:** I built a tiny tool that makes reading my AI coding agent's output actually calm

claude-review is a read-only review pane for Claude Code: one session, latest
response only, rendered as markdown in a split terminal. The pitch I landed on —
*faster than HTML, calmer than the terminal.* HTML reports for deep reads, this
for the fast/zen sweet spot in between.

~300 lines of Python, one dependency, MIT. First real release — would love
feedback on the idea and the README.

https://github.com/r3al1tymonster/claude-review

---

## 3. r/commandline

**Title:** A read-only TUI that pins one Claude Code session and renders only its latest response (`rich`)

Built this to scratch my own itch. It tails a single session's transcript and
renders the current response as markdown, re-anchored to top each turn instead
of scrolling. `Tab` switches surfaces (response/plan/tasks), `f` freezes the
view, a two-line muted footer carries all state — no header, nothing competing
with the text.

Strictly read-only and offline: reads transcript files, no writes, no network,
no telemetry. Single dependency is `rich`.

Source + demo gif: https://github.com/r3al1tymonster/claude-review
Happy to talk through the rendering/anchoring approach.

---

## 4. r/ChatGPTCoding   (flair: Project)

**Title:** [Project] claude-review — a zen, read-only pane for your AI coding session's latest answer

If you run an agentic coding CLI in the terminal, you know the output scrolls by
faster than you can read it. claude-review pins one session in a second pane and
shows just the latest response, rendered as markdown and refreshed in place — so
you can actually read and decide while the agent keeps working.

Built for Claude Code, read-only/offline, MIT.

Install: `npx skills add r3al1tymonster/claude-review -g`
Repo: https://github.com/r3al1tymonster/claude-review

---

## 5. r/ClaudeAI

**Title:** Reading Claude Code's output was stressing me out, so I built a calm second pane for it

The live terminal moves too fast to actually *read* a long answer, and asking
for an HTML report every time is overkill. So I made a tiny read-only pane that
pins one session and shows only its latest response, rendered as markdown and
refreshed in place. You read and decide in a quiet pane while Claude keeps
working in the first.

No writes, no network, no telemetry — it just reads the transcript files. MIT,
one dependency (`rich`).

https://github.com/r3al1tymonster/claude-review — would love to hear if this
fits how you work.
