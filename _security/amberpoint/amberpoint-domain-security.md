---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amberpoint.com
  spf: true
hosts:
- host: amberpoint.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amberpoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amberpoint, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Amberpoint
provider_slug: amberpoint
slug: amberpoint-domain-security
source_filename: amberpoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amberpoint.com\n  https: false\ndomains:\n- domain: amberpoint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amberpoint/refs/heads/main/security/amberpoint-domain-security.yml
summary_line: DMARC
tags:
- Company
- SOA
- API Management
- Governance
- Middleware
- Web Services
- Enterprise
- Acquired
---
