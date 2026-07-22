---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moat.com
  spf: false
hosts:
- host: moat.com
  https: false
kind: domain-security
layout: security
method: probed
name: Moat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moat, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Moat
provider_slug: moat
slug: moat-domain-security
source_filename: moat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moat.com\n  https: false\ndomains:\n- domain: moat.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moat/refs/heads/main/security/moat-domain-security.yml
summary_line: DMARC
tags:
- Company
- Advertising
- Analytics
- Ad Measurement
- Ad Viewability
- Brand Safety
- Marketing
- Acquired
---
