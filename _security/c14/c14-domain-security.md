---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: c14.money
  spf: true
hosts:
- host: c14.money
  https: false
kind: domain-security
layout: security
method: probed
name: C14 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for C14, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: C14
provider_slug: c14
slug: c14-domain-security
source_filename: c14-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: c14.money\n  https: false\ndomains:\n- domain: c14.money\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/c14/refs/heads/main/security/c14-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Fintech
- Crypto
- Payments
- On-Ramp
- Digital Assets
- Web3
---
