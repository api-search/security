---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stone.com.br
  spf: true
hosts:
- cert_expires: Aug  2 12:30:33 2026 GMT
  host: www.stone.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 11:09:47 2026 GMT
  host: online.stone.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 15:46:18 2026 GMT
  host: docs.openbank.stone.com.br
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stone, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stone
provider_slug: stone
slug: stone-domain-security
source_filename: stone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stone.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 12:30:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: online.stone.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 11:09:47 2026 GMT\n  hsts: null\n- host: docs.openbank.stone.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:46:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: stone.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stone/refs/heads/main/security/stone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Fintech
- Pix
- Brazil
- Digital Banking
- Payment Processing
- Boleto
- Financial Technology
---
