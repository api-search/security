---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sanadcash.com
  spf: true
hosts:
- host: sanadcash.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sanad Cash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sanad Cash, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sanad Cash
provider_slug: sanad-cash
slug: sanad-cash-domain-security
source_filename: sanad-cash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sanadcash.com\n  https: false\ndomains:\n- domain: sanadcash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanad-cash/refs/heads/main/security/sanad-cash-domain-security.yml
summary_line: DMARC
tags:
- Company
- Fintech
- Payments
- On-Demand Pay
- Earned Wage Access
- Saudi Arabia
- Acquired
---
