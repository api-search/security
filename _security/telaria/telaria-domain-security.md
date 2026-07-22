---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: telaria.com
  spf: true
hosts:
- cert_expires: Sep 15 17:25:07 2026 GMT
  host: telaria.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telaria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telaria, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Telaria
provider_slug: telaria
slug: telaria-domain-security
source_filename: telaria-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: telaria.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 17:25:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: telaria.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telaria/refs/heads/main/security/telaria-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Video Advertising
- Connected TV
- CTV
- Supply-Side Platform
- SSP
- Programmatic
- Acquired
---
