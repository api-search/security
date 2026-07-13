---
api_specs:
- filename: cronitor-monitors-api-openapi.yml
  format: yaml
  label: Cronitor Monitors API
  slug: monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronitor/refs/heads/main/openapi/cronitor-monitors-api-openapi.yml
- filename: cronitor-telemetry-api-openapi.yml
  format: yaml
  label: Cronitor Telemetry API
  slug: telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronitor/refs/heads/main/openapi/cronitor-telemetry-api-openapi.yml
- filename: cronitor-groups-notifications-api-openapi.yml
  format: yaml
  label: Cronitor Sites API
  slug: sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronitor/refs/heads/main/openapi/cronitor-groups-notifications-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cronitor.io
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: cronitor.link
  spf: false
hosts:
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: cronitor.io
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: cronitor.link
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cronitor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cronitor, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Cronitor
provider_slug: cronitor
slug: cronitor-domain-security
source_filename: cronitor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cronitor.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: false\n- host: cronitor.link\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cronitor.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: cronitor.link\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cronitor/refs/heads/main/security/cronitor-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Monitoring
- Cron Jobs
- Scheduled Tasks
- Alerting
- Uptime
- Telemetry
- Status Pages
---
