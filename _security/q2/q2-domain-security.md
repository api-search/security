---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: q2.com
  spf: true
hosts:
- cert_expires: Sep 16 08:21:50 2026 GMT
  host: docs.helix.q2.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 22:13:07 2026 GMT
  host: api.helix.q2.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Q2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Q2, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Q2
provider_slug: q2
slug: q2-domain-security
source_filename: q2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.helix.q2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:21:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.helix.q2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 22:13:07 2026 GMT\n  hsts: null\ndomains:\n- domain: q2.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/q2/refs/heads/main/security/q2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Banking
- Embedded Finance
- Banking as a Service
- FinTech
- Digital Banking
- Cards
- Payments
- ACH
- FDIC
---
