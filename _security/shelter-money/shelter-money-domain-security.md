---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shelter.money
  spf: true
hosts:
- cert_expires: Nov  3 21:51:00 2026 GMT
  host: shelter.money
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.shelter.money
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Shelter Money Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shelter, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shelter
provider_slug: shelter-money
slug: shelter-money-domain-security
source_filename: shelter-money-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shelter.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 21:51:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.shelter.money\n  https: false\ndomains:\n- domain: shelter.money\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shelter-money/refs/heads/main/security/shelter-money-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Personal Finance
- Budgeting
- Fintech
- MCP
- AI Agents
- Cash Flow Forecasting
---
