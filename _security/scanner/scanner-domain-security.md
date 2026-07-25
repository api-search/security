---
api_specs:
- filename: scanner-ad-hoc-queries-api-openapi.yml
  format: yaml
  label: Scanner Ad Hoc Queries API
  slug: scanner-ad-hoc-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanner/refs/heads/main/openapi/scanner-ad-hoc-queries-api-openapi.yml
- filename: scanner-detection-rules-api-openapi.yml
  format: yaml
  label: Scanner Detection Rules API
  slug: scanner-detection-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanner/refs/heads/main/openapi/scanner-detection-rules-api-openapi.yml
- filename: scanner-event-sinks-api-openapi.yml
  format: yaml
  label: Scanner Event Sinks API
  slug: scanner-event-sinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanner/refs/heads/main/openapi/scanner-event-sinks-api-openapi.yml
- filename: scanner-indexes-api-openapi.yml
  format: yaml
  label: Scanner Indexes API
  slug: scanner-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanner/refs/heads/main/openapi/scanner-indexes-api-openapi.yml
- filename: scanner-info-api-openapi.yml
  format: yaml
  label: Scanner Info API
  slug: scanner-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanner/refs/heads/main/openapi/scanner-info-api-openapi.yml
- filename: scanner-lookup-tables-api-openapi.yml
  format: yaml
  label: Scanner Lookup Tables API
  slug: scanner-lookup-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanner/refs/heads/main/openapi/scanner-lookup-tables-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scanner.dev
  spf: true
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: scanner.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scanner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scanner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scanner
provider_slug: scanner
slug: scanner-domain-security
source_filename: scanner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scanner.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scanner.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scanner/refs/heads/main/security/scanner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- SIEM
- Log Analytics
- Threat Detection
- Security Operations
- Observability
- MCP
---
