---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: podia.com
  spf: true
hosts:
- cert_expires: Oct  5 17:06:13 2026 GMT
  host: www.podia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 17:12:52 2026 GMT
  host: help.podia.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Podia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Podia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Podia
provider_slug: podia
slug: podia-domain-security
source_filename: podia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.podia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 17:06:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.podia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 17:12:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: podia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podia/refs/heads/main/security/podia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Creator Economy
- Online Courses
- Digital Products
- Memberships
- Email Marketing
- No Public API
- Zapier Only
---
