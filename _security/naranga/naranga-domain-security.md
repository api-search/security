---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: naranga.com
  spf: true
hosts:
- host: naranga.com
  https: false
kind: domain-security
layout: security
method: probed
name: Naranga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Naranga, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Naranga
provider_slug: naranga
slug: naranga-domain-security
source_filename: naranga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: naranga.com\n  https: false\ndomains:\n- domain: naranga.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/naranga/refs/heads/main/security/naranga-domain-security.yml
summary_line: DMARC
tags:
- Franchise Management
- Franchise Operations
- Lead Management
- CRM
- Training
- Field Audits
- Multi-Location
- SaaS
- No Public API
---
