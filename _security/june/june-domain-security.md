---
api_specs:
- filename: june-tracking-api-openapi.yml
  format: yaml
  label: June Tracking API
  slug: tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/june/refs/heads/main/openapi/june-tracking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: june.so
  spf: true
hosts:
- cert_expires: Sep 18 10:15:55 2026 GMT
  host: www.june.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.june.so
  https: false
- cert_expires: Sep 17 06:07:40 2026 GMT
  host: help.june.so
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: June Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for June, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: June
provider_slug: june
slug: june-domain-security
source_filename: june-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.june.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:15:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.june.so\n  https: false\n- host: help.june.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 06:07:40 2026 GMT\n  hsts: false\ndomains:\n- domain: june.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/june/refs/heads/main/security/june-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Product Analytics
- B2B SaaS
- Event Tracking
- Segment Compatible
- Retention
- Feature Adoption
- Activation
---
