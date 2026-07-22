---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sanlo.io
  spf: true
hosts:
- host: sanlo.io
  https: false
kind: domain-security
layout: security
method: probed
name: Sanlo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sanlo, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sanlo
provider_slug: sanlo
slug: sanlo-domain-security
source_filename: sanlo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sanlo.io\n  https: false\ndomains:\n- domain: sanlo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanlo/refs/heads/main/security/sanlo-domain-security.yml
summary_line: DMARC
tags:
- Company
- Entertainment
- Gaming
- Payments
- Monetization
- Checkout
- Fintech
- Games
- SDK
- Web Checkout
---
