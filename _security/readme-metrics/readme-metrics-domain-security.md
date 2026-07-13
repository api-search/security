---
api_specs:
- filename: 6733983cabaf62002c7b16d9
  format: yaml
  label: ReadMe API
  slug: readme-api
  spec_type: OpenAPI
  url: https://spec.readme.com/openapi/6733983cabaf62002c7b16d9
- filename: readme-metrics-openapi.yml
  format: yaml
  label: ReadMe Metrics
  slug: readme-metrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme-metrics/refs/heads/main/openapi/readme-metrics-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.com
  spf: true
hosts:
- cert_expires: Oct  6 16:29:30 2026 GMT
  host: readme.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 07:54:10 2026 GMT
  host: docs.readme.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 14:04:20 2026 GMT
  host: dash.readme.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Readme Metrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReadMe Metrics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ReadMe Metrics
provider_slug: readme-metrics
slug: readme-metrics-domain-security
source_filename: readme-metrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: readme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:29:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.readme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 07:54:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dash.readme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:04:20 2026 GMT\n  hsts: null\ndomains:\n- domain: readme.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/readme-metrics/refs/heads/main/security/readme-metrics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Analytics
- API Documentation
- API Logs
- API Metrics
- API Usage
- Developer Experience
- Developer Hubs
---
