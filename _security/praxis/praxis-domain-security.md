---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: praxisnation.com
  spf: true
hosts:
- cert_expires: Oct  9 14:24:48 2026 GMT
  host: www.praxisnation.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Praxis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Praxis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Praxis
provider_slug: praxis
slug: praxis-domain-security
source_filename: praxis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.praxisnation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:24:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: praxisnation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/praxis/refs/heads/main/security/praxis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real-Estate
- Smart Cities
- Communities
- Membership
- Urban Development
- Network State
---
