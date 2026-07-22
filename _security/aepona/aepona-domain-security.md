---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aepona.com
  spf: true
hosts:
- host: www.aepona.com
  https: false
kind: domain-security
layout: security
method: probed
name: Aepona Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aepona, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aepona
provider_slug: aepona
slug: aepona-domain-security
source_filename: aepona-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aepona.com\n  https: false\ndomains:\n- domain: aepona.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aepona/refs/heads/main/security/aepona-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Infrastructure
- Telecommunications
- APIs
- Network as a Service
- API Monetization
- Mobile
- Acquired
---
