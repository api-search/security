---
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Shelter Money Trust Center
name_suffix: Trust Center
overview: Shelter maintains a public trust center covering its security and compliance posture.
provider_name: Shelter
provider_slug: shelter-money
slug: shelter-money-trust-center
source_filename: shelter-money-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nprobe: true\nsource: https://shelter.money/security\nurl: https://shelter.money/security\ncertifications: []\nnote: >-\n  CORRECTED 2026-09-07: an automated keyword probe initially credited SOC 2, ISO 27001, and\n  HIPAA from this page, but the page names them only under a \"What we don't claim\" section —\n  Shelter explicitly states it is NOT certified for any of them. Recorded as an honest zero.\n  The page is a genuine security-practices disclosure: Plaid read-only access tokens encrypted\n  at rest (AES-256-GCM, random IV per token), passwords delegated to Clerk (Clerk-issued JWT,\n  no stored passwords), card details held by Stripe (Shelter stores only customer ID and\n  subscription status), TLS with HSTS/CSP/X-Frame-Options, and an architectural inability to\n  move money.\nevidence:\n- source: https://shelter.money/security\n  status: 200\n  note: SOC 2 / ISO 27001 / HIPAA appear under \"What we don't claim\" — explicitly\
  \ not certified\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shelter-money/refs/heads/main/security/shelter-money-trust-center.yml
summary_line: trust center published
tags:
- Personal Finance
- Budgeting
- Fintech
- MCP
- AI Agents
- Cash Flow Forecasting
trust_url: https://shelter.money/security
---
