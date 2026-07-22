---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shriramcity.in
  spf: true
hosts:
- host: www.shriramcity.in
  https: false
kind: domain-security
layout: security
method: probed
name: Shriram City Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shriram City, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shriram City
provider_slug: shriram-city
slug: shriram-city-domain-security
source_filename: shriram-city-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shriramcity.in\n  https: false\ndomains:\n- domain: shriramcity.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shriram-city/refs/heads/main/security/shriram-city-domain-security.yml
summary_line: DMARC
tags:
- Company
- Fintech
- NBFC
- Lending
- Consumer Finance
- Financial Services
- India
---
