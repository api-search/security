---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aaptiv.com
  spf: true
hosts:
- cert_expires: Aug 29 19:26:20 2026 GMT
  host: aaptiv.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aaptiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aaptiv, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aaptiv
provider_slug: aaptiv
slug: aaptiv-domain-security
source_filename: aaptiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aaptiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 19:26:20 2026 GMT\n  hsts: false\ndomains:\n- domain: aaptiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aaptiv/refs/heads/main/security/aaptiv-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Fitness
- Wellness
- Health
- Mobile
- AI Coaching
---
