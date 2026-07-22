---
api_specs:
- filename: notyfi-openapi-original.json
  format: json
  label: Notyfi API
  slug: notyfi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notyfi/refs/heads/main/openapi/notyfi-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: notyfi.com
  spf: true
hosts:
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: api.notyfi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Notyfi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Notyfi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Notyfi
provider_slug: notyfi
slug: notyfi-domain-security
source_filename: notyfi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.notyfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: notyfi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notyfi/refs/heads/main/security/notyfi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Notifications
- Monitoring
- Webhooks
- Real Time
- Agents
- MCP
- Alerts
---
