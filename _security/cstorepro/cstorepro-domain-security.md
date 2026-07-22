---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cstorepro.com
  spf: true
hosts:
- host: cstorepro.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cstorepro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CStorePro, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CStorePro
provider_slug: cstorepro
slug: cstorepro-domain-security
source_filename: cstorepro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cstorepro.com\n  https: false\ndomains:\n- domain: cstorepro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cstorepro/refs/heads/main/security/cstorepro-domain-security.yml
summary_line: DMARC
tags:
- Company
- Convenience Store
- Retail
- Point of Sale
- Back Office
- Fuel
- Scan Data
- Loyalty
- Financial Management
---
