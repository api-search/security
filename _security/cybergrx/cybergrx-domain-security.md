---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cybergrx.com
  spf: true
hosts:
- host: www.cybergrx.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cybergrx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CyberGRX, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CyberGRX
provider_slug: cybergrx
slug: cybergrx-domain-security
source_filename: cybergrx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cybergrx.com\n  https: false\ndomains:\n- domain: cybergrx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybergrx/refs/heads/main/security/cybergrx-domain-security.yml
summary_line: DMARC
tags:
- Company
- Cybersecurity
- Third Party Risk
- Vendor Risk Management
- Risk Management
- GRC
- Security Assessment
---
