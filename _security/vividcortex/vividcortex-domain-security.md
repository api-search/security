---
api_specs:
- filename: vividcortex-openapi.yml
  format: yaml
  label: VividCortex Database Performance Monitor API
  slug: vividcortex-database-performance-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vividcortex/refs/heads/main/openapi/vividcortex-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vividcortex.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: docs.vividcortex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: app.vividcortex.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vividcortex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VividCortex, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VividCortex
provider_slug: vividcortex
slug: vividcortex-domain-security
source_filename: vividcortex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.vividcortex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.vividcortex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: vividcortex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vividcortex/refs/heads/main/security/vividcortex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Database
- Performance Monitoring
- Observability
- Monitoring
- APM
- Database Performance
- SQL
- DevOps
- SolarWinds
---
