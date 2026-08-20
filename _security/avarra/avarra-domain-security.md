---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: avarra.ai
  spf: true
hosts:
- cert_expires: Sep 19 19:00:03 2026 GMT
  host: www.avarra.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: api.avarra.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avarra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avarra, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Avarra
provider_slug: avarra
slug: avarra-domain-security
source_filename: avarra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avarra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:00:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.avarra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: avarra.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avarra/refs/heads/main/security/avarra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sales Enablement
- Sales Training
- Artificial Intelligence
- Coaching
- Role-Play Simulation
- Revenue Operations
- Onboarding
- Sales Readiness
- Conversation Intelligence
---
