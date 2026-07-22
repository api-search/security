---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tangelolatam.com
  spf: true
hosts:
- host: www.tangelolatam.com
  https: false
kind: domain-security
layout: security
method: probed
name: Tangelo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tangelo, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tangelo
provider_slug: tangelo
slug: tangelo-domain-security
source_filename: tangelo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tangelolatam.com\n  https: false\ndomains:\n- domain: tangelolatam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tangelo/refs/heads/main/security/tangelo-domain-security.yml
summary_line: DMARC
tags:
- Company
- Fintech
- Financial Services
- Latin America
- LATAM
- Developer Portal
- API
- Status Page
---
