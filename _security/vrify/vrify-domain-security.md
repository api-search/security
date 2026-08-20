---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vrify.com
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: vrify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vrify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VRIFY, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: VRIFY
provider_slug: vrify
slug: vrify-domain-security
source_filename: vrify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vrify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vrify.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vrify/refs/heads/main/security/vrify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Mining
- Mineral Exploration
- Geoscience
- Artificial Intelligence
- Machine-Learning
- 3D Visualization
- Data Visualization
- Investor Relations
- Software-as-a-Service
- Canada
---
