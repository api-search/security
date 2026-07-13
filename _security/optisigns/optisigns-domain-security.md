---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: optisigns.com
  spf: true
hosts:
- cert_expires: Oct  1 11:31:02 2026 GMT
  host: www.optisigns.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 07:49:49 2026 GMT
  host: docs.optisigns.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: graphql-gateway.optisigns.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optisigns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OptiSigns, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OptiSigns
provider_slug: optisigns
slug: optisigns-domain-security
source_filename: optisigns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.optisigns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:31:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.optisigns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 07:49:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: graphql-gateway.optisigns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: optisigns.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optisigns/refs/heads/main/security/optisigns-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Signage
- Screens
- Content Management
- GraphQL
- Displays
- Playlists
---
