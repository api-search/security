---
api_specs:
- filename: helika-events-openapi.json
  format: json
  label: Helika Analytics Service
  slug: helika-analytics-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helika/refs/heads/main/openapi/helika-events-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: helika.io
  spf: true
hosts:
- cert_expires: Sep 21 15:56:01 2026 GMT
  host: www.helika.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 04:29:32 2026 GMT
  host: docs.helika.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: events.analytics.helika.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helika Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helika, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Helika
provider_slug: helika
slug: helika-domain-security
source_filename: helika-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helika.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:56:01 2026 GMT\n  hsts: false\n- host: docs.helika.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 04:29:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: events.analytics.helika.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: helika.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helika/refs/heads/main/security/helika-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Gaming
- Analytics
- Game Analytics
- Web3
- Events
- AI
- SDK
- Player Data
---
