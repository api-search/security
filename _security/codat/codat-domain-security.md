---
api_specs:
- filename: codat-platform-openapi.json
  format: json
  label: Codat Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat/refs/heads/main/openapi/codat-platform-openapi.json
- filename: codat-lending-openapi.json
  format: json
  label: Codat Lending API
  slug: lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat/refs/heads/main/openapi/codat-lending-openapi.json
- filename: codat-bank-feeds-openapi.json
  format: json
  label: Codat Bank Feeds API
  slug: bank-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat/refs/heads/main/openapi/codat-bank-feeds-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: codat.io
  spf: true
hosts:
- cert_expires: Aug 15 11:57:27 2026 GMT
  host: app.codat.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 19:25:16 2026 GMT
  host: docs.codat.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 11:57:27 2026 GMT
  host: api.codat.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codat, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Codat
provider_slug: codat
slug: codat-domain-security
source_filename: codat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.codat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 11:57:27 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.codat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 19:25:16 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.codat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 11:57:27 2026 GMT\n  hsts: null\ndomains:\n- domain: codat.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codat/refs/heads/main/security/codat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Unified_API
---
