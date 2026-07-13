---
api_specs:
- filename: better-stack-openapi.yml
  format: yaml
  label: Better Stack API
  slug: betterstack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/openapi/better-stack-openapi.yml
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
name: Betterstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Better Stack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Better Stack
provider_slug: betterstack
slug: betterstack-domain-security
source_filename: betterstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: betterstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 13:54:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63113904\n- host: uptime.betterstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 21:14:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63113904\ndomains:\n- domain: betterstack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betterstack/refs/heads/main/security/betterstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Observability
- Uptime Monitoring
- Incidents
- Logs
- Monitoring
- Status Pages
- On-Call
---
