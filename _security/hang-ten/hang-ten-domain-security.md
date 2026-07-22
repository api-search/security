---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hangten.ai
  spf: true
hosts:
- cert_expires: Sep 27 18:56:14 2026 GMT
  host: hangten.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hang Ten Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hang Ten, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hang Ten
provider_slug: hang-ten
slug: hang-ten-domain-security
source_filename: hang-ten-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hangten.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 18:56:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hangten.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hang-ten/refs/heads/main/security/hang-ten-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Enterprise Software
- AI Services
- Consulting
- Agentic AI
- SAP
---
