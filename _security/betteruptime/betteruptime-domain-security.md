---
api_specs:
- filename: betteruptime-uptime-api-openapi.yml
  format: yaml
  label: Better Stack Uptime API
  slug: uptime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betteruptime/refs/heads/main/openapi/betteruptime-uptime-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: betterstack.com
  spf: true
hosts:
- cert_expires: Oct  5 13:54:01 2026 GMT
  host: betterstack.com
  hsts: true
  hsts_max_age: 63113904
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 21:14:46 2026 GMT
  host: uptime.betterstack.com
  hsts: true
  hsts_max_age: 63113904
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Betteruptime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Better Uptime, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Better Uptime
provider_slug: betteruptime
slug: betteruptime-domain-security
source_filename: betteruptime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: betterstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 13:54:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63113904\n- host: uptime.betterstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 21:14:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63113904\ndomains:\n- domain: betterstack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betteruptime/refs/heads/main/security/betteruptime-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Uptime Monitoring
- Incident Management
- Status Pages
- On-Call Scheduling
- Observability
- DevOps
---
