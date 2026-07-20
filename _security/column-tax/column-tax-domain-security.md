---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: columntax.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: columnapi.com
  spf: false
hosts:
- cert_expires: Sep 12 19:13:30 2026 GMT
  host: www.columntax.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 13:46:45 2026 GMT
  host: docs.columntax.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: prod.columnapi.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Column Tax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Column Tax, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Column Tax
provider_slug: column-tax
slug: column-tax-domain-security
source_filename: column-tax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.columntax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 19:13:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.columntax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 13:46:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: prod.columnapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: columntax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: columnapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/column-tax/refs/heads/main/security/column-tax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Tax
- Tax Filing
- Embedded Finance
- E-File
- Financial Services
- Banking
- API First
---
