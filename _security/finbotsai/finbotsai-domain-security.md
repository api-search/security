---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: finbots.ai
  spf: true
hosts:
- cert_expires: Sep  9 16:37:50 2026 GMT
  host: finbots.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finbotsai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finbots.AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Finbots.AI
provider_slug: finbotsai
slug: finbotsai-domain-security
source_filename: finbotsai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finbots.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 16:37:50 2026 GMT\n  hsts: false\ndomains:\n- domain: finbots.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finbotsai/refs/heads/main/security/finbotsai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Credit Risk
- Credit Scoring
- Fintech
- Lending
- Banking
- Machine Learning
- Risk Management
- Singapore
---
