# Security Certification Roadmap

An interactive, opinionated visualization of the cybersecurity certification landscape — built for practitioners who want signal, not noise.

**Live demo:** open `Best.html` directly in any modern browser. No server, no dependencies, no install.

---

## What This Is

This is a single-file HTML tool that maps the security certification ecosystem across three lenses:

- **Wheel view** — certifications arranged in a radial chart by domain and skill tier
- **Training Quality** — organizations ranked by how well their training actually produces competent practitioners
- **HR vs. Community** — a scatter plot showing where employer demand and practitioner respect agree, diverge, or contradict

The ratings are firsthand and opinionated. No vendor paid to be here. No cert is included just because it exists — it's included because it matters to someone's career or the community has a strong opinion about it, positive or negative.

---

## Why the Domains Are Arranged the Way They Are

The wheel isn't random. Adjacent domains share meaningful overlap, and the layout reflects that:

**Network & Hacking → Web Security & Hacking**
Web attacks live on top of network fundamentals. SQL injection, SSRF, and API abuse all require understanding of how traffic moves. These two domains share the most practitioner crossover — someone doing network pentesting will inevitably touch web targets and vice versa.

**Web Security & Hacking → AI Security / Hacking**
AI systems are increasingly exposed as web APIs. Prompt injection, model endpoints, and LLM attack surfaces are fundamentally web attack surfaces with a new layer on top. An AppSec practitioner moving into AI offensive work is a natural progression, not a career change.

**AI Security / Hacking → Engineering / Exploit Dev**
Building adversarial ML tools, writing model theft exploits, or attacking agentic pipelines requires engineering depth — binary understanding, memory models, toolchain knowledge. The transition from AI offense into low-level exploit development is steep but logical for those going deep.

**Engineering / Exploit Dev → Governance & Risk**
Security architects and senior engineers eventually own risk decisions. The engineering domain bleeds into governance for those moving into leadership, architecture review, or compliance-adjacent roles in high-security environments.

**Governance & Risk → Audit & Compliance → Blue Team / SOC**
These three form the defensive and organizational spine of the wheel. Governance sets policy, audit verifies it, and the SOC enforces it operationally. They sit together because career paths flow naturally between them — a CISO draws on all three.

**Blue Team / SOC → Network & Hacking**
The wheel completes the circle here intentionally. The best defenders understand offense. SOC analysts who cross-train in network pentesting become dramatically more effective at detection, threat hunting, and incident response.

---

## How the Tier System Works

The five tiers map to both experience level and rough educational equivalence. This isn't a claim that certs equal degrees — it's a framework for understanding the depth of knowledge each tier represents.

| Tier | Color | Experience | Degree Equivalent |
|------|-------|------------|-------------------|
| Foundational | Gray | 0–2 years | Pre-degree / entry |
| Practical | Green | 2–4 years | Associate's Degree |
| Professional | Blue | 4–10 years | Bachelor's Degree |
| Expert | Amber | 10–20 years | Master's Degree |
| God Tier | Red | 20+ years | PhD |

**Center = rarest and hardest. Outer ring = most accessible.**

A God Tier cert like OSEE (OffSec Exploitation Expert) has fewer than a few dozen holders globally. A Foundational cert like Security+ has hundreds of thousands. Both have value — but they signal very different things.

---

## How the Scoring Works

Every certification and training organization is scored across three axes:

**Training Quality (T)** — Does the material actually make you better? Labs, depth, real-world applicability. This is the harshest score. A cert that teaches to the test scores low regardless of brand.

**HR / Employer Sentiment (E)** — Do hiring managers recognize and value it? Does it pass ATS filters? Is it on job postings? A cert can score high here even if practitioners don't respect it (CEH is the classic example).

**Community Respect (C)** — What do working practitioners think? Reddit, Discord, conference hallways, CTF circles. This is the signal that HR sentiment often lags by years.

The gap between E and C is where the most interesting information lives. A cert with high E and low C is a checkbox credential — valuable for getting past the initial screen, weak as a signal of actual skill. A cert with high C and low E is underrated and often worth targeting before the market catches up.

---

## No Chart Is Perfect

There is no objectively correct way to map a certification landscape. This tool reflects one practitioner's perspective, built from direct experience, community observation, and firsthand assessment of training quality across dozens of providers. Others will reasonably disagree on specific placements, scores, or domain assignments.

What makes this approach different:

- Tier placement is based on what the cert actually demands of the holder, not what the vendor claims
- Scoring is separated into three dimensions rather than collapsed into a single rating
- Domain adjacency reflects real career paths, not marketing categories
- Offensive certifications are explicitly flagged (⚔) because they require different legal and professional context
- Vendor-specific certifications (AWS, Azure, GCP, Cisco vendor-track, etc.) are intentionally excluded — this map covers third-party and vendor-neutral credentials only

---

## Files

| File | Description |
|------|-------------|
| `Best.html` | The complete interactive tool — single file, no dependencies |
| `README.md` | This file |
| `LICENSE` | MIT License |

---

## Usage

1. Clone or download the repo
2. Open `Best.html` in a browser
3. Use the tabs to switch between Certifications, Training Quality, and HR vs. Community views
4. Use domain filters to focus on a specific area
5. Hover any node for detail; click to open the certification's official page

---

## Contributing

Pull requests welcome for:
- New certifications that meet the inclusion bar (third-party/vendor-neutral, meaningful community or employer signal)
- URL corrections (exam pages move)
- Score updates backed by community evidence
- New training organizations

Please do not submit PRs to add vendor-specific certifications (AWS, Azure, GCP, Microsoft, Cisco product-track, etc.) — that scope is intentionally out of bounds.

---

## License

MIT — use it, fork it, build on it. Attribution appreciated but not required.
