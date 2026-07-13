---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tronox.com
  spf: true
hosts:
- cert_expires: Sep  9 17:33:35 2026 GMT
  host: www.tronox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.tronox.com
  https: false
- host: api.tronox.com
  https: false
kind: domain-security
layout: security
method: probed
name: Tronox Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tronox Holdings, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tronox Holdings
provider_slug: tronox-holdings
slug: tronox-holdings-domain-security
source_filename: tronox-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tronox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 17:33:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.tronox.com\n  https: false\n- host: api.tronox.com\n  https: false\ndomains:\n- domain: tronox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tronox-holdings/refs/heads/main/security/tronox-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Titanium Dioxide
- Chemical
- Mining
---
