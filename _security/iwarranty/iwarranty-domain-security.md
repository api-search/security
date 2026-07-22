---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iwarranty.co
  spf: true
hosts:
- cert_expires: Oct 15 08:07:27 2026 GMT
  host: iwarranty.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iwarranty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iwarranty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Iwarranty
provider_slug: iwarranty
slug: iwarranty-domain-security
source_filename: iwarranty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iwarranty.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 08:07:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iwarranty.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iwarranty/refs/heads/main/security/iwarranty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Warranty Management
- Claims Management
- Warranty
- Retail
- Manufacturing
- SaaS
- Sustainability
- Fraud Detection
---
