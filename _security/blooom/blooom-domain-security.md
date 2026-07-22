---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blooom.com
  spf: true
hosts:
- host: blooom.com
  https: false
kind: domain-security
layout: security
method: probed
name: Blooom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blooom, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blooom
provider_slug: blooom
slug: blooom-domain-security
source_filename: blooom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blooom.com\n  https: false\ndomains:\n- domain: blooom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blooom/refs/heads/main/security/blooom-domain-security.yml
summary_line: DMARC
tags:
- Company
- Wealth Management
- Retirement
- 401k
- Robo-Advisor
- Investing
- Fintech
- Defunct
---
