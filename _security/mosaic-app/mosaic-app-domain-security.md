---
api_specs:
- filename: mosaic-app-members-api-openapi.yml
  format: yaml
  label: Mosaic Members API
  slug: mosaic-app-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosaic-app/refs/heads/main/openapi/mosaic-app-members-api-openapi.yml
- filename: mosaic-app-projects-api-openapi.yml
  format: yaml
  label: Mosaic Projects API
  slug: mosaic-app-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosaic-app/refs/heads/main/openapi/mosaic-app-projects-api-openapi.yml
- filename: mosaic-app-tasks-api-openapi.yml
  format: yaml
  label: Mosaic Tasks API
  slug: mosaic-app-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosaic-app/refs/heads/main/openapi/mosaic-app-tasks-api-openapi.yml
- filename: mosaic-app-time-entries-api-openapi.yml
  format: yaml
  label: Mosaic Time Entries API
  slug: mosaic-app-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosaic-app/refs/heads/main/openapi/mosaic-app-time-entries-api-openapi.yml
- filename: mosaic-app-work-plans-api-openapi.yml
  format: yaml
  label: Mosaic Work Plans API
  slug: mosaic-app-work-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosaic-app/refs/heads/main/openapi/mosaic-app-work-plans-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mosaicapp.com
  spf: true
hosts:
- cert_expires: Aug 17 10:32:29 2026 GMT
  host: mosaicapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 01:52:51 2026 GMT
  host: readme.mosaicapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: api-server.prod.prod.us-east-1.mosaicapp.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mosaic App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mosaic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mosaic
provider_slug: mosaic-app
slug: mosaic-app-domain-security
source_filename: mosaic-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mosaicapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 10:32:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: readme.mosaicapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 01:52:51 2026 GMT\n  hsts: null\n- host: api-server.prod.prod.us-east-1.mosaicapp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mosaicapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mosaic-app/refs/heads/main/security/mosaic-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Resource Management
- Workforce Planning
- Project Management
- AEC
- Professional Services
- Time Tracking
- Forecasting
- AI Assistant
- Integration Platform
- Fortune 500
---
