---
api_specs:
- filename: garner-openapi-original.json
  format: json
  label: Garner Health API
  slug: garner-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/garner/refs/heads/main/openapi/garner-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getgarner.com
  spf: true
hosts:
- cert_expires: Aug 27 01:35:16 2026 GMT
  host: www.getgarner.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: api.getgarner.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Garner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Garner, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Garner
provider_slug: garner
slug: garner-domain-security
source_filename: garner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getgarner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 01:35:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getgarner.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: getgarner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/garner/refs/heads/main/security/garner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthtech
- Healthcare
- Provider Data
- Care Navigation
- Health Insurance
- Claims Analytics
- Provider Search
- Doctor Quality
---
