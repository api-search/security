---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: quintessent.com
  spf: true
hosts:
- cert_expires: Oct  6 15:38:23 2026 GMT
  host: quintessent.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quintessent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quintessent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Quintessent
provider_slug: quintessent
slug: quintessent-domain-security
source_filename: quintessent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quintessent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:38:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: quintessent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quintessent/refs/heads/main/security/quintessent-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Deep Tech
- Photonics
- Semiconductors
- Optical Interconnects
- Quantum Dot
- AI Infrastructure
- Hardware
---
