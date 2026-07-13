---
api_specs:
- filename: schoology-openapi.yml
  format: yaml
  label: Schoology REST API v1
  slug: rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-openapi.yml
- filename: schoology-webhooks-openapi.yml
  format: yaml
  label: Schoology Event Triggers (Webhooks) API
  slug: event-triggers-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-webhooks-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: schoology.com
  spf: true
hosts:
- cert_expires: Aug  4 00:22:56 2026 GMT
  host: www.schoology.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: developers.schoology.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api.schoology.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Schoology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Schoology, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Schoology
provider_slug: schoology
slug: schoology-domain-security
source_filename: schoology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.schoology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 00:22:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.schoology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\n- host: api.schoology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: schoology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/security/schoology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EdTech
- LMS
- K-12
---
