---
api_specs:
- filename: daycal-io-owner-api-openapi.yml
  format: yaml
  label: Daycal Owner API
  slug: daycal-io-owner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daycal-io/openapi/daycal-io-owner-api-openapi.yml
- filename: daycal-io-public-api-openapi.yml
  format: yaml
  label: Daycal Public API
  slug: daycal-io-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daycal-io/openapi/daycal-io-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: daycal.io
  spf: true
hosts:
- cert_expires: Jan  9 23:31:42 2027 GMT
  host: daycal.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Daycal Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daycal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Daycal
provider_slug: daycal-io
slug: daycal-io-domain-security
source_filename: daycal-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daycal.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:31:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: daycal.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/daycal-io/security/daycal-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Scheduling
- Calendar
- AI Assistant
- Productivity
- Automation
- Company
---
