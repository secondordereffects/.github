# Contributing to Second Order Effects

Thank you for your interest in contributing. This guide applies to all repositories under the [github.com/secondordereffects](https://github.com/secondordereffects) organization.

---

## Repositories

| Repository | What to Contribute |
|------------|-------------------|
| [`content`](https://github.com/secondordereffects/content) | New catalog entries, corrections, sources, cross-references |
| `secondordereffects.github.io` | Website features, bug fixes, accessibility, performance |

---

## Contributing Catalog Entries

### What We're Looking For

| Type | Description | Impact |
|------|-------------|--------|
| **New Entries** | Original analysis of second-order effects | HIGH |
| **Counter-Evidence** | Data that challenges existing entries | HIGH |
| **Quantification** | Adding numbers to qualitative claims | MEDIUM |
| **Sources** | Adding citations to existing entries | MEDIUM |
| **Cross-References** | Linking related effects | LOW |
| **Typo Fixes** | Corrections to text | LOW |

### Entry Quality Bar

Every new entry **must** include:

- [ ] **CHAIN Framework structure** — Context, Hypothesis, Actual Chain, Impact, Navigation
- [ ] **At least one quantified impact** — Numbers, not just words
- [ ] **At least one verifiable source** — Academic, industry report, or documented case study
- [ ] **Falsifiability criteria** — What would prove this wrong?
- [ ] **Actionable navigation** — What should readers do with this knowledge?

### The CHAIN Framework

```
C — Context       What's the situation? Who is making this decision?
H — Hypothesis    What's the expected first-order outcome?
A — Actual Chain  What second/third/nth order effects actually occur?
I — Impact        Quantified consequences (time, money, complexity)
N — Navigation    How to anticipate or mitigate
```

### Quick Start

Content contributions go to the [content repo](https://github.com/secondordereffects/content):

```bash
# Fork and clone the content repo
git clone https://github.com/YOUR_USERNAME/content.git
cd content

# Entries live in entries/<category>/<ID>/meta.json
# See the content repo README for the full schema
```

For engine/website contributions:

```bash
# Fork and clone both repos
git clone https://github.com/YOUR_USERNAME/secondordereffects.github.io.git
git clone https://github.com/YOUR_USERNAME/content.git

# Symlink content into engine
cd secondordereffects.github.io
ln -s ../content ./content

npm install
npm run dev
```

### Code Style

- TypeScript strict mode
- Prettier for formatting
- ESLint for linting
- Tailwind CSS for styling

---

## Evidence Standards

| Evidence Type | Acceptable | Not Acceptable |
|---------------|------------|----------------|
| Academic papers | ✅ | |
| Industry reports (Gartner, McKinsey, etc.) | ✅ | |
| Company case studies (documented) | ✅ | |
| Personal experience (labeled as such) | ✅ | |
| "I think" / "Everyone knows" | | ❌ |
| Unverifiable claims | | ❌ |

## Quantification Standards

| Good | Bad |
|------|-----|
| "+40% increase in team size over 18 months" | "Significant increase" |
| "P99 latency: 200ms → 800ms" | "Latency got worse" |
| "Range: 20-40% based on [source]" | "About 30%" (unsourced) |

---

## Commit Convention

```
type(scope): description

entry(T010): add Rewrite Fallacy analysis
fix(web): resolve D3 tree rendering on mobile
docs: update CHAIN framework explanation
```

Types: `entry`, `fix`, `docs`, `style`, `refactor`, `chore`

---

## Review Process

1. **Automated checks** — Template structure, link checking, spell checking
2. **Maintainer review** — CHAIN compliance, evidence quality, writing quality
3. **Community feedback** — 48-hour comment period for new entries
4. **Merge or revision** — Approved entries merged; others returned with feedback

---

## On AI-Assisted Contributions

**We welcome AI-assisted contributions.** Requirements:

- **Human verification of all claims** — AI hallucinates. You must verify.
- **Human verification of all sources** — Check that links work and say what you claim.
- **Disclosure if asked** — If someone asks "did you use AI?", be honest.

The value is in *insight quality*, not *production method*.

---

## License

By contributing, you agree that your contributions will be licensed under:
- **Content:** CC BY 4.0
- **Code:** MIT

---

## Questions?

- **Discussions:** [GitHub Discussions](https://github.com/secondordereffects/content/discussions)
- **Email:** [hello@lagbase.com](mailto:hello@lagbase.com)
- **Twitter:** [@lagaboratory](https://x.com/lagaboratory)
