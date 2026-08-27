## Ibrahim Litinine

I build go-to-market systems: the outbound workflows, the data plumbing behind
them, and the sites and content that explain them. Most of my work is one thing
end to end, design through to the code that ships it.

---

### What I work with

**GTM & outbound** · Clay · HubSpot · Salesforce · Apollo · Instantly ·
Smartlead · Lemlist · HeyReach · PhantomBuster · LinkedIn Sales Navigator

**Automation** · n8n · Make · Zapier · Airtable

**Build** · Framer (CMS, localization, custom embeds) · Webflow · JavaScript ·
Python · Node

**AI** · Claude / Anthropic API · OpenAI (image generation pipelines) ·
Claude Code and Agent Skills

---

### Things I have built

**Thirty interactive workflow charts, in a CMS**
Each workflow on [nebor.ai](https://nebor.ai) renders a clickable diagram: a
step rail, a detail panel, tool tooltips, a walkthrough that steps card by
card. Each ships as a **self-contained embed** — every icon, font fallback and
image inlined — because the host renders it inside a sandboxed iframe with no
external requests. Bilingual EN/NL from one source, picking its language from
the URL. One template, thirty items, a build that regenerates all of them, and
**ten automated gates** that run before anything ships.

**A build that refuses to ship a known failure**
The trickiest bug on that project was invisible: the CMS flattens every newline
to a space, so a surviving `//` comment eats the rest of the script and leaves
a program that *compiles clean and renders nothing*. `node --check` cannot see
it. The build now counts line comments and fails on them, so it cannot happen
twice.

**Content at volume, with a quality bar that is executable**
169 GTM glossary entries edited to a documented voice standard, plus long-form
articles. The editorial rules are not a style guide anyone has to remember:
they are a script that fails the build.

**Image pipelines**
75 article image projects and roughly 4,200 generated images through a
repeatable OpenAI pipeline: a locked visual language, cost controls, and
quality checks, rather than one-off prompting.

**Codified process as tooling**
Nine [Agent Skills](https://docs.claude.com/en/docs/claude-code/skills) that
capture how each kind of work gets done — article writing, editorial passes,
workflow page design and copy, image and badge generation — so the standard is
reproducible instead of living in my head.

---

### How I work

- **Verify, don't assert.** If I say it works, I measured it. Most of the bugs
  worth catching were the ones that looked fine.
- **Make the standard executable.** A rule in a document gets forgotten; a gate
  in the build does not.
- **Fix the cause.** The symptom is usually a layer above where the problem is.
- **Say what I skipped.** Partial work reported as finished costs more than the
  work saved.

---

Most repositories here are private client work. Happy to walk through any of it.

📫 [nebor.ai](https://nebor.ai)
