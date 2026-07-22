---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: abacum.io
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: www.abacum.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abacum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abacum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Abacum
provider_slug: abacum
slug: abacum-domain-security
source_filename: abacum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abacum.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: abacum.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abacum/refs/heads/main/security/abacum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Saas
- FP&A
- Financial Planning
- Finance
- Budgeting
- Forecasting
- CFO
- Reporting
- Integrations
---
