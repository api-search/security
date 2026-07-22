---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: collabra.ai
  spf: true
hosts:
- cert_expires: Sep  6 17:15:27 2026 GMT
  host: collabra.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Collabra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Collabra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Collabra
provider_slug: collabra
slug: collabra-domain-security
source_filename: collabra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: collabra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 17:15:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: collabra.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collabra/refs/heads/main/security/collabra-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Enterprise
- Automation
- Artificial Intelligence
- RPA
- Compliance
- Back Office
- SaaS
- Australia
---
