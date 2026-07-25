---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pnfp.com
  spf: true
hosts:
- cert_expires: Aug  6 21:18:29 2026 GMT
  host: www.pnfp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pinnacle Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pinnacle Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pinnacle Financial
provider_slug: pinnacle-financial
slug: pinnacle-financial-domain-security
source_filename: pinnacle-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pnfp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  6 21:18:29 2026 GMT\n  hsts: null\ndomains:\n- domain: pnfp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinnacle-financial/refs/heads/main/security/pinnacle-financial-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Services
- Banking
- United States
- Regional Bank
- Open Finance
- Data Aggregation
---
