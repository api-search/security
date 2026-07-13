---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vetspire.com
  spf: true
hosts:
- cert_expires: Sep 21 02:19:20 2026 GMT
  host: vetspire.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 14:40:16 2026 GMT
  host: developer.vetspire.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 21:54:45 2026 GMT
  host: api.vetspire.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vetspire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vetspire, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vetspire
provider_slug: vetspire
slug: vetspire-domain-security
source_filename: vetspire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vetspire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 02:19:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.vetspire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:40:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: api.vetspire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 21:54:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vetspire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vetspire/refs/heads/main/security/vetspire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Veterinary
- Practice Management
- PIMS
- Healthcare
- GraphQL
- Electronic Medical Records
- Scheduling
---
