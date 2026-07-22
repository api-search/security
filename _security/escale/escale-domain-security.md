---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: escale.ai
  spf: false
hosts:
- cert_expires: Sep  7 19:45:02 2026 GMT
  host: escale.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Escale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Escale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Escale
provider_slug: escale
slug: escale-domain-security
source_filename: escale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: escale.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 19:45:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: escale.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/escale/refs/heads/main/security/escale-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Sales
- Artificial Intelligence
- Customer Acquisition
- Conversational AI
- Marketing
- Brazil
- Fintech
---
