---
api_specs:
- filename: monoscope-platform-openapi.yml
  format: yaml
  label: Monoscope Platform API
  slug: monoscope-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apitoolkit/refs/heads/main/openapi/monoscope-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: monoscope.tech
  spf: true
hosts:
- cert_expires: Sep 13 05:01:30 2026 GMT
  host: monoscope.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 19:26:14 2026 GMT
  host: api.monoscope.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apitoolkit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIToolkit (Monoscope), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: APIToolkit (Monoscope)
provider_slug: apitoolkit
slug: apitoolkit-domain-security
source_filename: apitoolkit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monoscope.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 05:01:30 2026 GMT\n  hsts: false\n- host: api.monoscope.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 19:26:14 2026 GMT\n  hsts: null\ndomains:\n- domain: monoscope.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apitoolkit/refs/heads/main/security/apitoolkit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Observability
- API Analytics
- API Catalog
- API Management
- API Monitoring
- API Testing
- Breaking Change Detection
- CLI
- Debugging
- Error Tracking
- LLM Observability
- Logs and Traces
- MCP Server
- Metrics
- Monitors
- Observability
- OpenTelemetry
- Platform
- Session Replay
---
