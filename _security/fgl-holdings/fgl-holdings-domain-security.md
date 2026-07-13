---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fglife.com
  spf: true
hosts:
- cert_expires: Aug 14 11:13:49 2026 GMT
  host: www.fglife.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.fglife.com
  https: false
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: api.fglife.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fgl Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FGL Holdings, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FGL Holdings
provider_slug: fgl-holdings
slug: fgl-holdings-domain-security
source_filename: fgl-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fglife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 11:13:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.fglife.com\n  https: false\n- host: api.fglife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fglife.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fgl-holdings/refs/heads/main/security/fgl-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Annuities
- Financial Services
---
