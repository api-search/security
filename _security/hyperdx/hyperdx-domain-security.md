---
api_specs:
- filename: hyperdx-external-api-openapi.json
  format: json
  label: HyperDX External API
  slug: hyperdx-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperdx/refs/heads/main/openapi/hyperdx-external-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hyperdx.io
  spf: true
hosts:
- cert_expires: Oct  4 01:45:58 2026 GMT
  host: www.hyperdx.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api.hyperdx.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperdx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HyperDX, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HyperDX
provider_slug: hyperdx
slug: hyperdx-domain-security
source_filename: hyperdx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hyperdx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:45:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hyperdx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hyperdx.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperdx/refs/heads/main/security/hyperdx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Observability
- Monitoring
- Logging
- Tracing
- Metrics
- OpenTelemetry
- ClickHouse
- Open Source
- Alerting
- Dashboards
- Session Replay
- Developer Tools
- Agents
---
