---
layout: post
title: "Nvidia Jetson Naming: A Masterclass in Confusion"
date: 2025-08-15
description: How to make a perfectly good hardware lineup unnecessarily complicated
tags: technote
categories: Algoblog
giscus_comments: false
related_posts: false
related_publications: true
toc:
  sidebar: left
---

*How to make a perfectly good hardware lineup unnecessarily complicated*

## The Problem

Nvidia is worth $4.3 trillion and dominates AI hardware. You'd expect their product naming to be crystal clear. Instead, the Jetson lineup reads like a tangled airline route map.

If you're a CTO in Osaka staring at a procurement spreadsheet, you might find yourself asking: "Is Orin Nano faster than Xavier NX?" The answer requires diving into spec sheets, architecture whitepapers, and forum archaeology. This shouldn't be hard.

For a company whose valuation depends on being indispensable, the naming scheme seems designed to keep customers confused just long enough to click through more comparison charts. The messiness appears to be a feature, not a bug.

## The Lineup That Ate Clarity

The current Jetson family includes: Nano, Orin Nano, Orin NX, AGX Orin, Xavier NX, AGX Xavier, and the upcoming Thor. These names don't follow a clear performance hierarchy or generational progression. Xavier NX might be weaker or stronger than Orin Nano depending entirely on which architecture generation you're comparing. {% cite arif2025deep %}, {% cite swaminathan2025benchmarking %}

### The Nano Problem

The original Nano was a $99 dev kit running basic YOLO detection - perfect for robotics clubs and hobby projects. Then came the Orin Nano with Ampere architecture and 40 TOPS of AI performance, capable of real-time multi-stream inference. Instead of retiring the old name or creating a clear distinction, Nvidia kept "Nano" for both. Now "Nano" means either "entry-level" or "mid-tier powerhouse" depending on which generation you're discussing.

### The NX Problem

NX supposedly represents the middle tier - more powerful than Nano, less than AGX. But Nvidia has never explained what "NX" stands for. It appears in both Xavier (Volta) and Orin (Ampere) generations, creating situations where an Orin NX (100 TOPS) vastly outperforms an AGX Xavier (32 TOPS). Any rational naming scheme would at least indicate generation. Instead, NX functions as a password to an exclusive club - useful only if you already know the lineage.

### The AGX Problem

AGX is the flagship tier. AGX Xavier (2018) was a 32 TOPS Volta-powered workhorse used in mining trucks and surgical robots. AGX Orin (2022) is a 275 TOPS Ampere-powered platform that handles large transformer models without thermal throttling. Both are just "AGX," despite representing a generational leap in capability. Nvidia has never publicly defined what AGX means - the leading theory from engineering forums suggests "Accelerated Graphics eXtension," though this may be a backronym.

### The Generation Problem

Orin and Xavier started as internal codenames but got promoted to customer-facing branding. This forces buyers to memorize architectural lineage. Orin uses newer GPU cores, faster tensor processing, and better power efficiency. Xavier is thermally constrained and requires INT8 quantization for modern YOLO models. These differences have real deployment consequences, yet the naming provides no hint.

### The Thor Problem

Thor targets humanoid robotics and will likely spawn Thor Nano, Thor NX, and AGX Thor variants. The pattern continues - none of these names will indicate which platform can actually power your prototype without thermal issues. The only way to know is to navigate to Nvidia's comparison matrix, where you'll conveniently encounter upsell opportunities.

## The Fix (They Won't Do It)

The solution is straightforward:

- **Clear tiering**: Jetson Lite, Jetson Pro, Jetson Max
- **Release years**: Pro 2025 vs Pro 2023 - immediately obvious which is newer
- **Reserve codenames**: Keep Orin, Xavier, Thor in engineering documentation where they belong
- **Consistent definitions**: "Nano" should always mean entry-level, not "depends on the year"

But Nvidia's naming chaos has become a deliberate funnel. The confusion drives engineers to product comparison pages loaded with benchmark charts and proprietary acronyms, effectively locking them into the ecosystem. It's a sales tactic implemented in silicon.

## Appendix: Jetson Comparison Reference

| Model | Released | GPU Arch | TOPS | Power | Notes |
|------------|--------|-----------------|-----------|------------|-------|
| Nano | 2019 | Maxwell | 0.5 | 5-10W | Legacy - don't start new projects |
| Orin Nano | 2023 | Ampere | 40 | 7-15W | Entry tier, current generation |
| Xavier NX | 2020 | Volta | 21 | 10-15W | Mid-tier, previous generation |
| Orin NX | 2023 | Ampere | 100 | 10-25W | Mid-tier, current generation |
| AGX Xavier | 2018 | Volta | 32 | 10-30W | Flagship, previous generation |
| AGX Orin | 2022 | Ampere | 275 | 15-60W | Flagship, current generation |

**Reading notes:**
- **TOPS** = Theoretical peak performance (like your car's top speed downhill with a tailwind)
- **Maxwell/Volta** = Don't deploy new projects on these architectures
- **Ampere (Orin/Thor)** = Current generation, recommended for new deployments
- The "Notes" column exists because Nvidia's naming reveals less than it should

---

**Footnotes:**

[1] Jetson modules are edge AI computers designed for on-site deployment - inside camera housings on factory floors or onboard delivery drones rather than in distant data centers.

[2] Both Nanos run TensorRT-optimized models. The Orin Nano just does it without thermal throttling.

[3] If AGX truly means "Accelerated Graphics eXtension," there's presumably a naming archive somewhere at Nvidia HQ with rejected alternatives like "Turbo Compute Pro" and "GigaVision Xtreme."
