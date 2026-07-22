---
api_specs:
- filename: superlog-management-openapi.json
  format: json
  label: Superlog Management API
  slug: superlog-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superlog/refs/heads/main/openapi/superlog-management-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: superlog.sh
  spf: true
hosts:
- cert_expires: Sep 27 17:40:26 2026 GMT
  host: docs.superlog.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: api.superlog.sh
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superlog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superlog, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Superlog
provider_slug: superlog
slug: superlog-domain-security
source_filename: superlog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.superlog.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:40:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.superlog.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: superlog.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superlog/refs/heads/main/security/superlog-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Observability
- OpenTelemetry
- Monitoring
- Logging
- Tracing
- Metrics
- Incident Management
- AI Agents
- Model Context Protocol
- Developer Tools
---
