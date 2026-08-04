---
title: Backflip — Generator Provenance
permalink: /generator-provenance
---

# Workout Generator — Training-Data Provenance

_Last reviewed: 2026-07-22_

## Summary

Backflip's workout generator is **100% rules-based**. There is **no trained
machine-learning model, no LLM, and no training dataset** behind plan
generation.

## What actually generates plans

- `WorkoutPlanGenerator` — deterministic, hand-authored rules.
- `PlanContext` — gathers the user's own signals (7-day muscle coverage,
  training rhythm, readiness deload, body-metric gentling) that those rules
  read.

All plan output is derived from (a) these hand-authored rules and (b) the
user's own logged data. No third-party proprietary or branded training
methodology is reproduced.

## Regulatory note (DPIIT, India)

India's DPIIT has proposed a mandatory blanket-licensing framework for AI
**training data**. Exposure here is **low**: there is no training data because
there is no trained model.

## Markets

Consent and disclosures are applied **universally** — the same acceptance gate
and the same disclosures are shown to every user regardless of region (the
DPDP + GDPR/ePrivacy + CCPA superset), so no market-specific carve-out is
needed for the generator.

## Revisit trigger

If an LLM or any trained/ML model is added, training-data IP provenance will be
re-evaluated **before** it ships.
