---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ricursive.com
  spf: false
hosts:
- cert_expires: Aug 27 22:50:46 2026 GMT
  host: ricursive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ricursive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ricursive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Ricursive
provider_slug: ricursive
slug: ricursive-domain-security
source_filename: ricursive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ricursive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 22:50:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ricursive.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ricursive/refs/heads/main/security/ricursive-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Chip Design
- Semiconductors
- Electronic Design Automation
- AI Lab
---
