---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modulehousing.com
  spf: true
hosts:
- cert_expires: Aug 26 04:03:18 2026 GMT
  host: modulehousing.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Module Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Module, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Module
provider_slug: module
slug: module-domain-security
source_filename: module-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modulehousing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 04:03:18 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: modulehousing.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/module/refs/heads/main/security/module-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Housing
- Construction
- Manufacturing
- Modular
- Real Estate
- Sustainability
---
