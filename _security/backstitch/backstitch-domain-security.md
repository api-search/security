---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: backstitch.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: backstit.ch
  spf: true
hosts:
- cert_expires: Oct  1 12:45:43 2026 GMT
  host: www.backstitch.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 13:57:49 2026 GMT
  host: docs.backstit.ch
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api.backstit.ch
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Backstitch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for backstitch, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: backstitch
provider_slug: backstitch
slug: backstitch-domain-security
source_filename: backstitch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.backstitch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 12:45:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.backstit.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 13:57:49 2026 GMT\n  hsts: null\n- host: api.backstit.ch\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: backstitch.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: backstit.ch\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backstitch/refs/heads/main/security/backstitch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Content Curation
- Employee Communications
- Internal Communications
- Total Rewards
- Content Aggregation
- Newsletters
- Widgets
- REST
---
