---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: moveitpro.com
  spf: true
- caa:
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zapier.com
  spf: true
hosts:
- cert_expires: Sep  7 06:45:31 2026 GMT
  host: www.moveitpro.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: zapier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moveitpro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoveitPro, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MoveitPro
provider_slug: moveitpro
slug: moveitpro-domain-security
source_filename: moveitpro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moveitpro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 06:45:31 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: zapier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: moveitpro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: zapier.com\n  dnssec: false\n  caa:\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moveitpro/refs/heads/main/security/moveitpro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Moving Software
- Moving Company
- Logistics
- Field Service
- Dispatch
- CRM
- Vertical SaaS
---
