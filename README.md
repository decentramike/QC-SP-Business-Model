# QC-SP Business Model — Project Charter

## Purpose

This tool exists to give Filecoin Storage Providers (SPs) a rigorous, forward-looking view of their economic position — before network changes take effect, before capital is committed, and before the market moves. It translates protocol-level proposals into P&L impact so that decisions are grounded in numbers, not assumptions.

Link [here](https://decentramike.github.io/QC-SP-Business-Model/)
---

## Objectives

### 1. Understand the SP Price Impact of Network Changes

Filecoin's revenue model is sensitive to a small set of variables: block reward rates, datacap multipliers, pledge requirements, and gas costs. Even modest parameter shifts can meaningfully change break-even timelines, ROI, and whether a given hardware configuration is viable.

**What this objective drives:**
- A configurable simulation engine that accepts any combination of parameter overrides
- Delta cards on every key metric (revenue, pledge, gas, break-even) showing current vs. proposed values
- Hardware tier modeling so SPs can match their physical configuration to projected returns
- Scenario comparison to evaluate competing proposals side by side

**Success looks like:** An SP can answer *"If this FIP passes, does my operation remain profitable — and at what FIL price does it stop being?"* in under five minutes.

---

### 2. Identify Interest in Direct Storage Deals

The Filecoin+ program (datacap / notary system) is one pathway to verified deals, but it is not the only one. Direct storage arrangements — where clients contract with SPs outside the notary flow — represent an underexplored opportunity.

**What this objective drives:**
- Modeling a "direct storage" revenue stream alongside block rewards
- Surfacing deal margin separately from network rewards so deal attractiveness is visible
- Tracking which network changes make direct storage *more* or *less* competitive relative to datacap-gated rewards

**Success looks like:** A clear view of the conditions under which direct storage deals improve overall SP economics, and a benchmark rate for what a deal would need to pay to be worth taking.

---

### 3. Proactively Monitor FIP Impact on SP Network ROI

FIPs are proposed continuously, often with long discussion periods before activation. SPs that wait until implementation to assess impact miss the window to adapt — operationally, contractually, and financially.

**What this objective drives:**
- A live FIP registry with pre-mapped parameter overrides for every proposal under active discussion
- Automatic delta computation so each FIP's effect on the SP's modeled operation is visible at a glance
- Status tracking (draft, active, final) so proposals can be prioritized by urgency
- Notifications-ready architecture to surface high-impact proposals as they progress

**Success looks like:** When a FIP moves from draft to last call, the SP already knows its projected P&L impact and has a position on it — not because they had to model it from scratch, but because the tool did.

---

## Current FIP Coverage

| FIP | Title | Status | Key Impact |
|-----|-------|--------|------------|
| FIP-0076 | Direct Data Onboarding | Active | Lower gas, reduced onboarding friction |
| FIP-0084 | Remove Datacap from Duration Multiplier | Draft | Partial datacap reduction |
| FIP-Daybreak | Restore Equal Sector Quality & Burn Mining Reserve | Draft | Eliminates 10x datacap premium; CC reward +8.5x; pledge +6.5x |

---

## Scope

This model covers the economics of a single SP operation. It does not model:
- Network-wide equilibrium effects (e.g., how total QAP changes as SPs respond)
- Token price dynamics from the mining reserve burn
- Governance or voting outcomes

Those factors matter, but they belong in a separate layer of analysis. This tool is for the SP deciding whether and how to operate — not for protocol designers modeling aggregate behavior.

---

## Stack

Single-file React app (`index.html`) — no build step, no backend, runs entirely in the browser. Hosted via GitHub Pages. All parameters are configurable at runtime.
