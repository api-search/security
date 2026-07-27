---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: totogi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: totogi.solutions
  spf: false
hosts:
- cert_expires: Oct  1 15:19:10 2026 GMT
  host: totogi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: docs.whoosh.totogi.solutions
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api.whoosh.totogi.solutions
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Totogi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Totogi, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Totogi
provider_slug: totogi
slug: totogi-domain-security
source_filename: totogi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: totogi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 15:19:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.whoosh.totogi.solutions\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: false\n- host: api.whoosh.totogi.solutions\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: totogi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: totogi.solutions\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/totogi/refs/heads/main/security/totogi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- United States
- BSS
- OSS
- Charging
- Messaging
- SMS
- A2P
- 5G
- TM Forum
- Standards
- Network Vendor
- Vertical AI
- GraphQL
- Policy Control
---
