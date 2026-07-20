---
api_specs:
- filename: base-operations-openapi-original.json
  format: json
  label: Base Operations Customer API
  slug: base-operations-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: baseoperations.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: baseoperationsenterprise.com
  spf: false
hosts:
- cert_expires: Sep 11 05:01:36 2026 GMT
  host: www.baseoperations.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.baseoperationsenterprise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Base Operations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Base Operations, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Base Operations
provider_slug: base-operations
slug: base-operations-domain-security
source_filename: base-operations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.baseoperations.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:01:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.baseoperationsenterprise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: baseoperations.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: baseoperationsenterprise.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/security/base-operations-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Threat Intelligence
- Security
- Risk Management
- Physical Security
- Crime Data
- Geospatial
- Public Safety
- Risk Scoring
---
