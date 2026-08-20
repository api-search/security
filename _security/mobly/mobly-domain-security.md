---
api_specs:
- filename: mobly-rest-api-v0-openapi.yml
  format: yaml
  label: Mobly REST API v0
  slug: mobly-rest-api-v0
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobly/refs/heads/main/openapi/mobly-rest-api-v0-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getmobly.com
  spf: true
hosts:
- cert_expires: Oct 15 21:23:50 2026 GMT
  host: www.getmobly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 21:11:47 2026 GMT
  host: help.getmobly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 01:48:34 2026 GMT
  host: core-api.getmobly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mobly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mob.ly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mob.ly
provider_slug: mobly
slug: mobly-domain-security
source_filename: mobly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getmobly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 21:23:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.getmobly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 21:11:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: core-api.getmobly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 01:48:34 2026 GMT\n  hsts: false\ndomains:\n- domain: getmobly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mobly/refs/heads/main/security/mobly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Event
- Event Marketing
- Lead Capture
- Lead Enrichment
- B2B
- Marketing
- Go-To-Market
- Artificial Intelligence
- CRM
- Marketing Automation
- Trade Shows
---
