---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: array.com
  spf: true
hosts:
- cert_expires: Oct  9 13:24:59 2026 GMT
  host: array.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Array Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Array, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Array
provider_slug: array
slug: array-domain-security
source_filename: array-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: array.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:24:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: array.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/array/refs/heads/main/security/array-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Embedded Finance
- Credit Data
- Identity
- Background Checks
- Credit Monitoring
- Consumer Data
- Financial Services
- API
---
