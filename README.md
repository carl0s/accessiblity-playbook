# accessiblity-playbook
Multi-book accessibility knowledge base as a Claude Code / Amp skill — distills the AccessAbility Playbook, Giving a Damn About Accessibility, and the Appt Handbook into on-demand frameworks for service, design, and WCAG/mobile.

## Install as a Claude Code skill

The skill lives in `SKILL.md` (with supporting content in `chapters/`, `glossary.md`, `patterns.md`, and `cheatsheet.md`). To use it in Claude Code, copy this repo into a skills directory under the skill's name (`accessability-playbook`).

### Personal skill (available in every project)

```bash
git clone https://github.com/<your-org>/accessiblity-playbook.git \
  ~/.claude/skills/accessability-playbook
```

Or, if you already have the repo checked out:

```bash
mkdir -p ~/.claude/skills
cp -R /path/to/accessiblity-playbook ~/.claude/skills/accessability-playbook
```

### Project skill (shared with a single repo)

```bash
mkdir -p .claude/skills
cp -R /path/to/accessiblity-playbook .claude/skills/accessability-playbook
```

Commit `.claude/skills/accessability-playbook/` so teammates get it automatically.

### Verify and use

1. Restart Claude Code (or run `/doctor`) so it picks up the new skill.
2. Run `/skills` (or ask "what skills do you have?") and confirm `accessability-playbook` is listed.
3. Invoke it by asking an accessibility question, or pass a topic/chapter directly, e.g. `appt-ch03`, a WCAG criterion, or a framework name.

> The directory name must match the `name:` field in `SKILL.md` (`accessability-playbook`). Claude Code loads any folder containing a `SKILL.md` from `~/.claude/skills/` (personal) or `.claude/skills/` (project).

## Contributing

**This is a collaborative project — PRs are more than welcome!** 🙌

The goal is a living, multi-source accessibility knowledge base. If you know a great resource — a book, handbook, standard, guideline, research paper, or practical pattern — please open a PR to integrate it. When adding a new source, credit the original author(s) and cite the work's license (see below), and only include material whose license permits redistribution.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full guide.

## License

This work is licensed under [**Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**](https://creativecommons.org/licenses/by-sa/4.0/) — see [LICENSE](LICENSE).

CC BY-SA 4.0 is required here (rather than a more permissive license) to comply with the **ShareAlike** obligation of the Appt Accessibility Handbook, whose content is itself CC BY-SA 4.0. Any redistribution or adaptation of this knowledge base must therefore keep the same license and preserve attribution to all original sources listed below — including a visible link to <https://appt.org>.

> Note: *Giving a Damn About Accessibility* is **not** distributed under an open-content license. It is summarized here (not reproduced verbatim) with attribution; this repo's CC BY-SA 4.0 license covers the original distillation, **not** the underlying work. Please refer to the author's terms before reusing material derived from it.

## Credits & source licenses

This knowledge base distills and is built upon the work of others. All credit for the underlying material goes to the original authors and publishers. Their works are reused here in line with their respective licenses; please honor those terms (including attribution) in any further reuse.

- **AccessAbility Playbook** — by **ESDC, Centre of Expertise for Accessible Client Service (Government of Canada)**. Crown Copyright © His Majesty the King in Right of Canada; Government of Canada material is generally made available for reuse under the [Open Government Licence – Canada](https://open.canada.ca/en/open-government-licence-canada). Source: <https://ceacs-cesca.github.io/playbook/>.
- **Giving a Damn About Accessibility** — by **Sheri Byrne-Haber, CPACC**. © Sheri Byrne-Haber. Distributed free of charge by the author (PDF + audiobook); it does not carry an explicit open-content license, so please refer to the author's terms before redistributing. Source: <https://www.accessibility.uxdesign.cc/>.
- **Appt Accessibility Handbook** — by the **Appt Foundation**. Content licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) and code under the [MIT license](https://opensource.org/licenses/MIT); attribution requires a visible link to <https://appt.org>. Source: <https://appt.org/en/handbook>.

> Note on licenses: where a source uses a ShareAlike or restrictive license, any redistribution (including this repo's derived summaries) must comply with the original terms. If you believe content here misattributes or misuses a source, please open an issue and it will be corrected promptly.
