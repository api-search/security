---
api_specs:
- filename: quodd-snapshots-api-openapi.yml
  format: yaml
  label: QUODD Snap API
  slug: quodd-snap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/openapi/quodd-snapshots-api-openapi.yml
- filename: quodd-snapshots-api-openapi.yml
  format: yaml
  label: QUODD Batch Snaps API
  slug: quodd-batch-snaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/openapi/quodd-snapshots-api-openapi.yml
- filename: quodd-options-api-openapi.yml
  format: yaml
  label: QUODD Options Snaps API
  slug: quodd-options-snaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/openapi/quodd-options-api-openapi.yml
- filename: quodd-authentication-api-openapi.yml
  format: yaml
  label: QUODD Authentication Token API
  slug: quodd-authentication-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/openapi/quodd-authentication-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quodd.com
  spf: true
hosts:
- cert_expires: Oct 10 02:12:11 2026 GMT
  host: www.quodd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: developer.quodd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.quodd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quodd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QUODD, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: QUODD
provider_slug: quodd
slug: quodd-domain-security
source_filename: quodd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quodd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 02:12:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.quodd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.quodd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quodd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/security/quodd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Market Data
- Real-Time Data
- Financial Data
- Streaming
- Historical Data
- Reference Data
- Quotes
- Fintech
---
