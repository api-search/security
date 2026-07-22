---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: atrisa.ai
  spf: true
hosts:
- cert_expires: Aug 29 05:15:54 2026 GMT
  host: atrisa.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atrisa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atrisa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Atrisa
provider_slug: atrisa
slug: atrisa-domain-security
source_filename: atrisa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atrisa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 05:15:54 2026 GMT\n  hsts: false\ndomains:\n- domain: atrisa.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atrisa/refs/heads/main/security/atrisa-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Analog Circuit Design
- EDA
- Semiconductors
- AI Agents
- Hardware Design
- Simulation
- Y Combinator
---
