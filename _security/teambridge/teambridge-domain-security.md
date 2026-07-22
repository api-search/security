---
api_specs:
- filename: teambridge-openapi-original.json
  format: json
  label: Teambridge External API
  slug: teambridge-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teambridge/refs/heads/main/openapi/teambridge-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: teambridge.com
  spf: true
hosts:
- cert_expires: Sep  8 21:09:08 2026 GMT
  host: teambridge.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: open-api.teambridge.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Teambridge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teambridge, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Teambridge
provider_slug: teambridge
slug: teambridge-domain-security
source_filename: teambridge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teambridge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 21:09:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: open-api.teambridge.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: teambridge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teambridge/refs/heads/main/security/teambridge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Workforce Management
- Scheduling
- Time Tracking
- Payroll
- HR
- Frontline
- Webhooks
---
