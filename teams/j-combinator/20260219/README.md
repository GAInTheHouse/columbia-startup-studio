# 20260219 — Product Brief, Brand Position & Synthetic User Testing

## What's in here

| File | Description |
|------|-------------|
| `product_brief.md` | One-page product brief — what we're building, who it's for, the core problem |
| `brand_position.md` | Internal brand positioning document — thesis, identity, canonical language |
| `synthetic_testing/` | 5 rounds of synthetic user testing on our V1 landing page copy |

## Synthetic Testing

We ran synthetic user testing using the [synthetic-user-testing skill](https://github.com/kenxle/columbia-startup-studio/tree/main/synthetic-user-testing) against landing page copy built from 10 real user interviews.

**Audience:** 60 AI-generated personas across 5 behavioral archetypes drawn from our interview data:

1. **Overwhelmed Planner** — decision fatigue, uses 3-6 platforms, "planning friend"
2. **Routine Breaker** — socially active but stuck in habit loops, wants novelty
3. **Quiet Explorer** — intentional, skeptical of hype, quality-over-quantity
4. **Culture Seeker** — wants ephemeral cultural events, frustrated by information asymmetry
5. **Budget-Conscious Socializer** — cost-aware, wants quality free/cheap activities

**Rounds:**

| Version | Copy file | Results | Key change |
|---------|-----------|---------|------------|
| V1 | `v1_copy.md` | `v1_results.md` | Initial copy from interviews |
| V2 | `v2_copy.md` | `v2_results.md` | Added example cards, elevated budget filter, algorithmic transparency line |
| V3 | `v3_copy.md` | `v3_results.md` | Reframed hero for routine breakers, added group planning mention |
| V4 | `v4_copy.md` | `v4_results.md` | Reworked social proof with beta-tester language, privacy line for quiet explorers |
| V5 | `v5_copy.md` | `v5_results.md` | Tightened CTA, added launch timeline, final polish |

### Extra files

`extra_files/v1/` through `extra_files/v5/` contain the full evaluation artifacts for each round: audience JSON, raw results JSON, charts (HTML), and detailed summaries. These aren't required but are included for reference.

```
extra_files/
├── v1/
│   ├── audience.json
│   ├── results_v1.json
│   ├── charts_v1.html
│   └── summary_v1.md
├── v2/
│   ├── copy_v2.md
│   ├── copy_v2_changes.md
│   ├── results_v2.json
│   ├── charts_v2.html
│   └── summary_v2.md
└── v5/
    └── ...
```

## Process

1. Drafted product brief and brand position using interview synthesis + LLM assistance, then edited for accuracy and voice
2. Wrote V1 landing page copy grounded in interview pain points and brand positioning
3. Generated 60 synthetic personas from interview archetypes (deterministic skeleton + qualitative enrichment)
4. Ran baseline evaluation against generic copy to calibrate the floor
5. Iterated V1 → V5 based on per-round feedback, tracking changes and rationale between versions
