---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cardiogram.com
  spf: true
hosts:
- host: cardiogram.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cardiogram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardiogram, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cardiogram
provider_slug: cardiogram
slug: cardiogram-domain-security
source_filename: cardiogram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cardiogram.com\n  https: false\ndomains:\n- domain: cardiogram.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardiogram/refs/heads/main/security/cardiogram-domain-security.yml
summary_line: DMARC
tags:
- Company
- Health
- Healthcare
- Digital Health
- Wearables
- Heart Rate
- Cardiovascular
- Machine Learning
- Consumer Health
---
