---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: josys.com
  spf: true
hosts:
- cert_expires: Aug 17 14:17:53 2026 GMT
  host: www.josys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 19:37:31 2026 GMT
  host: developer.josys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Josys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Josys, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Josys
provider_slug: josys
slug: josys-domain-security
source_filename: josys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.josys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 14:17:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.josys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:37:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: josys.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/josys/refs/heads/main/security/josys-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IT Asset Management
- SaaS Management
- Identity
- Device Management
---
