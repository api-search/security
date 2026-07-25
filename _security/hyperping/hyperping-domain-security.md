---
api_specs:
- filename: hyperping-healthchecks-api-openapi.yml
  format: yaml
  label: Hyperping Healthchecks API
  slug: hyperping-healthchecks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/openapi/hyperping-healthchecks-api-openapi.yml
- filename: hyperping-incidents-api-openapi.yml
  format: yaml
  label: Hyperping Incidents API
  slug: hyperping-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/openapi/hyperping-incidents-api-openapi.yml
- filename: hyperping-maintenance-api-openapi.yml
  format: yaml
  label: Hyperping Maintenance API
  slug: hyperping-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/openapi/hyperping-maintenance-api-openapi.yml
- filename: hyperping-monitors-api-openapi.yml
  format: yaml
  label: Hyperping Monitors API
  slug: hyperping-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/openapi/hyperping-monitors-api-openapi.yml
- filename: hyperping-outages-api-openapi.yml
  format: yaml
  label: Hyperping Outages API
  slug: hyperping-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/openapi/hyperping-outages-api-openapi.yml
- filename: hyperping-reports-api-openapi.yml
  format: yaml
  label: Hyperping Reports API
  slug: hyperping-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/openapi/hyperping-reports-api-openapi.yml
- filename: hyperping-status-pages-api-openapi.yml
  format: yaml
  label: Hyperping Status Pages API
  slug: hyperping-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/openapi/hyperping-status-pages-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hyperping.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: hyperping.io
  spf: true
hosts:
- cert_expires: Sep  1 01:06:13 2026 GMT
  host: hyperping.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 07:43:45 2026 GMT
  host: api.hyperping.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperping Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperping, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hyperping
provider_slug: hyperping
slug: hyperping-domain-security
source_filename: hyperping-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hyperping.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 01:06:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hyperping.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 07:43:45 2026 GMT\n  hsts: null\ndomains:\n- domain: hyperping.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: hyperping.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperping/refs/heads/main/security/hyperping-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Uptime Monitoring
- Status Pages
- Incident Management
- Observability
- On-Call
---
