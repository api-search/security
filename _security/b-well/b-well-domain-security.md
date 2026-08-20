---
api_specs:
- filename: b-well-users-api-openapi.yml
  format: yaml
  label: b.well Users API
  slug: b-well-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b-well/refs/heads/main/openapi/b-well-users-api-openapi.yml
- filename: b-well-webhook-api-openapi.yml
  format: yaml
  label: b.well Webhook API
  slug: b-well-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b-well/refs/heads/main/openapi/b-well-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: icanbwell.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: bwell.com
  spf: true
hosts:
- cert_expires: Oct 18 03:12:15 2026 GMT
  host: www.icanbwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 03:37:55 2026 GMT
  host: developer.bwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: api.client-sandbox.icanbwell.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: B Well Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for b.well, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: b.well
provider_slug: b-well
slug: b-well-domain-security
source_filename: b-well-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.icanbwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 03:12:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.bwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 03:37:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.client-sandbox.icanbwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: icanbwell.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bwell.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/b-well/refs/heads/main/security/b-well-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Healthcare
- Digital Health
- FHIR
- Health Data
- Interoperability
- Patient Access
- Health Records
- MCP
---
