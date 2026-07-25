---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: simplii.com
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: www.simplii.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Simplii Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simplii Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Simplii Financial
provider_slug: simplii-financial
slug: simplii-financial-domain-security
source_filename: simplii-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.simplii.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: simplii.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplii-financial/refs/heads/main/security/simplii-financial-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Canada
- Digital Bank
- Direct Banking
- Big Six
- CIBC
- Consumer-Driven Banking
- Data Aggregation
---
