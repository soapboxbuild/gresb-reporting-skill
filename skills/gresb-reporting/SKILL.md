---
name: gresb-reporting
description: Prepare GRESB Real Estate Assessment submissions, calculate scores, identify improvement opportunities, and generate GRESB-compliant ESG reports. Use when asked about GRESB, ESG scoring, institutional reporting, real estate sustainability benchmarking, or green star ratings.
---

## Assessment Type — Ask First

Real Estate Assessment or Infrastructure Assessment? These are completely different methodologies — do not mix.

## 2024 Pillar Weights (Real Estate Assessment)

**Management: 35%**
- Leadership (14 pts): senior executive commitment, board oversight, accountability
- Policies (10 pts): ESG policy scope, external assurance, stakeholder engagement
- Reporting (6 pts): public disclosure, external assurance of data
- Risk Management (5 pts): climate risk assessment, business plan integration

**Performance: 65%**
- Energy, GHG, Water, Waste: consumption data by asset
- Building Certifications: LEED, BREEAM, NABERS, etc.

## Data Coverage — Highest-Leverage Variable

Performance score is multiplied by **data coverage rate** = verified floor area / total portfolio floor area.

A portfolio with 40% coverage gets **at most 40%** of available Performance points, regardless of how good the verified data is. Surface this immediately when reviewing a GRESB portfolio — increasing coverage is always the first optimization.

**Score uplift priority order:**
1. Increase verified/covered floor area (multiplier effect)
2. Add green building certifications (LEED Gold = significant points)
3. Third-party assurance of energy/emissions data
4. Board-level ESG governance documentation
5. Reduce energy intensity year-over-year (trending matters)

## Submission Window

Submission: **April–July** each year. Reference year = prior calendar year. Flag if user is asking about submitting outside this window.

# GRESB Real Estate Assessment

## Overview
GRESB assesses real estate portfolios on Environmental, Social, and Governance performance. Results benchmark against global peers. Submission window: April-July annually.

## Score Structure
Total score = Management (30%) + Performance (70%)

### Management Component (30 pts)
- Leadership: ESG strategy, targets, executive oversight
- Policies: Environmental, social, anti-corruption
- Reporting: Public disclosure, third-party assurance
- Risk management: Climate risk, physical/transition

### Performance Component (70 pts)
**Coverage (data completeness):**
- Energy: electricity + fuel consumption by asset (kWh, GJ)
- GHG: Scope 1 + Scope 2 emissions (tCO2e) — methodology required
- Water: Municipal + other sources (m³)
- Waste: Total + diversion rate (tonnes)

**Like-for-Like (LfL) changes:** Year-over-year comparison of same-boundary assets

**Targets:** Absolute or intensity-based, science-aligned preferred

## Data Requirements by Asset Type

### Office/Retail/Industrial (Landlord-controlled areas):
- Base building energy: all common areas, HVAC, lighting
- Tenant energy: if available (green leases help)
- GHG conversion: use IEA or national grid emission factors
- Water: irrigation, cooling towers, common areas

### Multifamily Residential:
- Common area energy mandatory
- In-unit encouraged (smart meters)
- Water: full building if possible

## Scoring Tips
- Third-party verification adds 5-10 pts
- Green building certifications (LEED, BREEAM, ENERGY STAR) score in Management
- Science-based targets (SBTi) score highest for target quality
- Tenant engagement programs score in Social component
- Green leases: document and count toward tenant coverage

## GRESB Green Star Rating
- 1-5 stars based on total score + score relative to peers
- 5-star: top quintile AND score ≥ 70
- Green Star (any): score ≥ 50 + top 3 quintiles

## Key GRESB Terminology
- LfL: Like-for-Like boundary (stable assets only, no acquisitions/disposals)
- Absolute: Total portfolio consumption
- Intensity: Per m² or per occupant
- Landlord/Tenant control: who pays the utility bill
- Asset types: Office, Retail, Industrial, Residential, Hotel, Diversified

## Reporting Evidence
Document everything: utility invoices, meter data, certification certificates, policy documents, board minutes approving ESG strategy

## MCP Tools (requires GRESB Official Partner API access)
- `list_entities` — list GRESB entities you have access to
- `get_entity` — entity details
- `get_assessment_scores` — total/management/performance scores + green star rating
- `get_benchmark` — scores vs peer group median and top quartile
- `get_indicators` — indicator-level scores for management or performance
- `get_peer_comparison` — entity rank among peers
- `submit_indicator` — submit survey responses programmatically

To get API access: apply at gresb.com as an Official Data Partner.
In Soapbox: Settings → Plugins → GRESB Reporting → Add key (your GRESB API token).
