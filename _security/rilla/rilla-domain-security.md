---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rilla.com
  spf: true
- caa: []
  dmarc: true
  dmarc_pct: 25
  dmarc_policy: reject
  dnssec: false
  domain: rillavoice.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: apirilla.com
  spf: false
hosts:
- cert_expires: Oct  9 16:10:37 2026 GMT
  host: www.rilla.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 20:03:18 2026 GMT
  host: app.rilla.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: api.rillavoice.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  note: production API host; every /api/v1/* path answers 401 "Invalid Token"
  tls_version: TLSv1.3
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: api.apirilla.com
  hsts: false
  https: true
  note: AWS API Gateway; webhook receiver used by the SPOTIO integration
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rilla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rilla, probed live across 4 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rilla
provider_slug: rilla
slug: rilla-domain-security
source_filename: rilla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the Rilla API hosts discovered\n  in the app.rilla.com JavaScript bundle (api.rillavoice.com) and in the SPOTIO\n  integration documentation (api.apirilla.com)\nhosts:\n- host: www.rilla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:10:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.rilla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 20:03:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.rillavoice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  note: production API host; every /api/v1/* path answers 401 \"Invalid Token\"\n- host: api.apirilla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: false\n  note: AWS API Gateway; webhook receiver used by\
  \ the SPOTIO integration\ndomains:\n- domain: rilla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rillavoice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_pct: 25\n- domain: apirilla.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rilla/refs/heads/main/security/rilla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Conversation Intelligence
- Sales
- Coaching
- Sales Enablement
- Speech Analytics
- Machine-Learning
---
