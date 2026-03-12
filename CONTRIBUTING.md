# Contributing to Awesome CLI Tools & Apps

Thank you for taking the time to contribute! This is a **mega repository** bringing together **700+ command-line tools** from multiple curated sources ([awesome-shell](https://github.com/alebcay/awesome-shell), [awesome-cli-apps](https://github.com/agarrharr/awesome-cli-apps)) plus original contributions. This guide is a community resource and every improvement makes it more valuable for everyone.

---

## Table of Contents

- [Ways to Contribute](#ways-to-contribute)
- [Before You Open a PR](#before-you-open-a-pr)
- [Adding a New Tool](#adding-a-new-tool)
- [Fixing an Existing Entry](#fixing-an-existing-entry)
- [Table Format Reference](#table-format-reference)
- [Choosing the Right Section](#choosing-the-right-section)
- [Quality Checklist](#quality-checklist)
- [Pull Request Process](#pull-request-process)
- [What Will Be Rejected](#what-will-be-rejected)

---

## Ways to Contribute

| Type | Example |
| --- | --- |
| **Add a tool** | A CLI utility not yet in the guide |
| **Fix an error** | Wrong license, dead link, outdated version badge |
| **Improve a description** | Clearer wording, better use cases |
| **Update a section** | Tools moved to a better category |
| **Report an issue** | Open a GitHub Issue for anything you can't fix yourself |

---

## Before You Open a PR

1. **Check for duplicates.** Search the README for the tool name before adding it.
2. **Verify everything yourself.** Do not add what you have not personally tested or thoroughly researched. No guessing on licenses or repository URLs.
3. **One tool per PR is preferred.** Smaller, focused PRs are reviewed faster and are easier to accept or reject cleanly.

---

## Adding a New Tool

### Eligibility criteria

A tool is eligible if it meets **all** of the following:

- Runs from a terminal / command line (not a GUI app).
- Is actively maintained **or** is historically significant and widely installed.
- Has a public repository or official project page.
- Is free to use (open source, freeware, or meaningful free tier).

### Required information

For each new entry you must provide:

| Field | What to include |
| --- | --- |
| **Name** | Official name, linked to the homepage or docs |
| **Summary** | One sentence — what is the single most useful thing this tool does? |
| **Description** | 2–4 sentences. Key features and typical use cases. No marketing language. |
| **OS** | `All`, `Lin / mac`, `Lin`, `Win`, or `mac` (see abbreviations below) |
| **Repository** | Link text is `owner/repo`; URL points to the GitHub/GitLab/etc. page |
| **Latest Version** | Use a `shields.io` GitHub Release badge if the tool is on GitHub (see format below) |
| **License** | SPDX identifier (e.g. `MIT`, `Apache-2.0`, `GPL-3.0`) |
| **Open Source** | `✅` if OSI-approved license · `❌` if proprietary · `⚠️` if source-available but non-OSI |

**OS Abbreviations:**
- `All` — Windows, Linux, and macOS
- `Lin / mac` — Linux and macOS (no native Windows support)
- `Win` — Windows only
- `Lin` — Linux only
- `mac` — macOS only

**Version badge format (GitHub-hosted tools):**

```markdown
![GitHub Release](https://img.shields.io/github/v/release/OWNER/REPO?label=)
```

Use `—` for tools not on GitHub or without a tagged release.

---

## Fixing an Existing Entry

If you find a factual error (wrong license, archived project, broken link, incorrect OS support):

1. Open a **GitHub Issue** first if the fix is non-trivial, so it can be discussed.
2. For straightforward fixes (dead link, typo), a direct PR is fine.
3. In the PR description, explain what was wrong and link to the source that proves the correct value (e.g. link to the LICENSE file in the repo).

---

## Table Format Reference

All entries follow this column order:

```markdown
| Name | Summary | Description | OS | Repository | Latest Version | License | Open Source |
|------|---------|-------------|:--:|------------|:--------------:|---------|:-----------:|
| [Tool](https://homepage) | One-line summary | Detailed 2–4 sentence description. | All | [owner/repo](https://github.com/owner/repo) | ![GitHub Release](https://img.shields.io/github/v/release/owner/repo?label=) | MIT | ✅ |
```

Note the alignment markers:
- `OS` column: `:--:` (centered)
- `Latest Version` column: `:--------------:` (centered)
- `Open Source` column: `:-----------:` (centered)

---

## Choosing the Right Section

| Section | Belongs here if… |
| --- | --- |
| **Shell & Navigation** | Enhances the shell experience itself (prompt, history, navigation, env management) |
| **File & Directory Management** | Replaces or extends `ls`, `cat`, `find`, `du`, `df`, or file managers |
| **Search & Text Processing** | Searches inside files, transforms structured data, inspects binary/log files |
| **System Monitoring & Performance** | Monitors CPU, memory, disk, network, or processes |
| **Network & Web Tools** | Makes requests, scans networks, tests APIs, diagnoses connectivity |
| **Downloaders & Media** | Downloads video, audio, images, or galleries from online platforms |
| **Media Processing** | Processes images/video, renders visuals in-terminal, generates/reads QR codes |
| **Terminal Music & Audio Players** | Plays music, visualizes audio, reads RSS/podcasts |
| **Containers & Orchestration** | Manages Docker, Kubernetes, or other container runtimes |
| **Git & Development Tools** | Enhances git workflows, benchmarks, file watchers, compression, encryption |
| **Text Editors** | Terminal-based text editors (vim, emacs, nano alternatives) |
| **Productivity & Tasks** | Task management, journaling, note-taking, dashboards, presentations |
| **Databases & Data** | Database clients, query tools, data management utilities |
| **Security & Privacy** | Security scanning, encryption, password management, privacy tools |
| **Terminal Multiplexers** | Adds sessions, split panes, and window management inside any terminal |
| **Fun & Miscellaneous** | ASCII art, animations, eye candy, novelties |
| **Command Line Learning** | Interactive tutorials, cheat sheets, and CLI learning resources |

If unsure, suggest a section in your PR description and the maintainer will decide.

---

## Quality Checklist

Before submitting, verify every item:

- [ ] Tool name is spelled and capitalized correctly.
- [ ] Homepage link is the **official** site (not a mirror or third-party page).
- [ ] Repository link is the **official** upstream (not a fork).
- [ ] License identifier is a valid [SPDX expression](https://spdx.org/licenses/) or clearly stated.
- [ ] OS field accurately reflects **native** support (WSL does not count as Windows).
- [ ] Description contains **no invented features** — everything stated can be verified.
- [ ] Version badge URL uses the correct `owner/repo` from the repository link.
- [ ] The tool is **not archived** or unmaintained without being historically notable.

---

## Pull Request Process

1. Fork the repository and create a branch named `add/tool-name` or `fix/description`.
2. Make your changes following the format above.
3. Open a Pull Request with:
   - A clear title (e.g. `Add: bandwhich — per-process network monitor`)
   - A short description of what you added or fixed and why it belongs here.
4. The maintainer will review and may request changes or clarification.
5. Once approved, the PR will be merged and you will be credited in the commit history.

---

## What Will Be Rejected

The following will not be accepted:

- **Proprietary tools** with no meaningful free tier.
- **Abandoned projects** with no activity in 3+ years (unless historically significant).
- **Duplicate entries** — if a tool is already listed under a different name.
- **Inaccurate data** — wrong license, fake repository, invented features.
- **Self-promotion** without genuine merit — a tool must be useful to the community, not just a personal project.
- **AI-generated descriptions** that are vague, inaccurate, or not independently verified.

---

## License of Contributions

By submitting a Pull Request, you agree that your contribution will be published under the same [CC BY 4.0](LICENSE.md) license as the rest of this guide.
