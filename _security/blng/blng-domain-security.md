---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blng.ai
  spf: true
hosts:
- cert_expires: Sep 16 08:46:03 2026 GMT
  host: blng.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blng Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blng, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blng
provider_slug: blng
slug: blng-domain-security
source_filename: blng-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blng.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:46:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blng.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/security/blng-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Jewelry
- Generative AI
- Design
- Creative Tools
- Rendering
- Marketing
- Retail
---
