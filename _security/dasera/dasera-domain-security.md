---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dasera.com
  spf: true
hosts:
- host: dasera.com
  https: false
kind: domain-security
layout: security
method: probed
name: Dasera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dasera, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dasera
provider_slug: dasera
slug: dasera-domain-security
source_filename: dasera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dasera.com\n  https: false\ndomains:\n- domain: dasera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dasera/refs/heads/main/security/dasera-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Security
- Data Security
- Data Security Posture Management
- Data Governance
- Cloud Security
- Compliance
- Privacy
---
