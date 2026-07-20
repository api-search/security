---
api_specs:
- filename: goodays-openapi-original.json
  format: json
  label: Goodays API
  slug: goodays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodays/refs/heads/main/openapi/goodays-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: goodays.co
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: goodays.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 13:27:15 2026 GMT
  host: apidocs.goodays.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: api.goodays.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goodays Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goodays, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Goodays
provider_slug: goodays
slug: goodays-domain-security
source_filename: goodays-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goodays.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\n- host: apidocs.goodays.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 13:27:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.goodays.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: goodays.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodays/refs/heads/main/security/goodays-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Experience
- Customer Feedback
- Voice of the Customer
- Surveys
- NPS
- Reviews
- Retail
- CRM
- SaaS
---
