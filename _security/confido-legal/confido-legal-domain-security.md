---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: confidolegal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gravity-legal.com
  spf: true
hosts:
- cert_expires: Oct  8 04:17:44 2026 GMT
  host: confidolegal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 06:33:56 2026 GMT
  host: docs.confidolegal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: api.gravity-legal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Confido Legal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Confido Legal, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Confido Legal
provider_slug: confido-legal
slug: confido-legal-domain-security
source_filename: confido-legal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: confidolegal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 04:17:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.confidolegal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 06:33:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gravity-legal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: confidolegal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gravity-legal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confido-legal/refs/heads/main/security/confido-legal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compliance
- Disbursements
- GraphQL
- IOLTA
- Law
- LawTech
- Legal
- Legal Technology
- Payments
- Trust Accounting
---
