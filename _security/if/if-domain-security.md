---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: integrated.finance
  spf: true
hosts:
- cert_expires: Oct 14 22:17:36 2026 GMT
  host: integrated.finance
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 03:09:30 2026 GMT
  host: developer.integrated.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  3 12:04:44 2026 GMT
  host: api.integrated.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: If Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IF, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IF
provider_slug: if
slug: if-domain-security
source_filename: if-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: integrated.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:17:36 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: developer.integrated.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 03:09:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.integrated.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 12:04:44 2026 GMT\n  hsts: null\ndomains:\n- domain: integrated.finance\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/if/refs/heads/main/security/if-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Embedded Finance
- Banking as a Service
- Payments
- Cards
- Foreign Exchange
- Compliance
- Open Banking
- API
---
