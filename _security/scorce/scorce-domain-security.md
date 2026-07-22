---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scorce.io
  spf: true
hosts:
- host: scorce.io
  https: false
kind: domain-security
layout: security
method: probed
name: Scorce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scorce, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Scorce
provider_slug: scorce
slug: scorce-domain-security
source_filename: scorce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scorce.io\n  https: false\ndomains:\n- domain: scorce.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scorce/refs/heads/main/security/scorce-domain-security.yml
summary_line: DMARC
tags:
- Company
- KYC
- Identity Verification
- Fraud Prevention
- Authentication
- API Aggregator
- Fintech
- LatAm
---
