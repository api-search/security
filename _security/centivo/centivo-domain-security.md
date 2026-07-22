---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: centivo.com
  spf: true
hosts:
- cert_expires: Sep 16 22:29:50 2026 GMT
  host: centivo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Centivo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centivo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Centivo
provider_slug: centivo
slug: centivo-domain-security
source_filename: centivo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: centivo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 22:29:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: centivo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centivo/refs/heads/main/security/centivo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health Insurance
- Health Plans
- Employee Benefits
- Self-Funded
- Primary Care
---
