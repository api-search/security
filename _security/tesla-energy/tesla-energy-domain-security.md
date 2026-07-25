---
api_specs:
- filename: tesla-energy-backup-api-openapi.yml
  format: yaml
  label: Tesla Energy Backup API
  slug: tesla-energy-backup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-backup-api-openapi.yml
- filename: tesla-energy-history-api-openapi.yml
  format: yaml
  label: Tesla Energy History API
  slug: tesla-energy-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-history-api-openapi.yml
- filename: tesla-energy-live-status-api-openapi.yml
  format: yaml
  label: Tesla Energy Live Status API
  slug: tesla-energy-live-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-live-status-api-openapi.yml
- filename: tesla-energy-off-grid-charging-api-openapi.yml
  format: yaml
  label: Tesla Energy Off Grid Charging API
  slug: tesla-energy-off-grid-charging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-off-grid-charging-api-openapi.yml
- filename: tesla-energy-operation-api-openapi.yml
  format: yaml
  label: Tesla Energy Operation API
  slug: tesla-energy-operation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-operation-api-openapi.yml
- filename: tesla-energy-products-api-openapi.yml
  format: yaml
  label: Tesla Energy Products API
  slug: tesla-energy-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-products-api-openapi.yml
- filename: tesla-energy-programs-api-openapi.yml
  format: yaml
  label: Tesla Energy Programs API
  slug: tesla-energy-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-programs-api-openapi.yml
- filename: tesla-energy-site-info-api-openapi.yml
  format: yaml
  label: Tesla Energy Site Info API
  slug: tesla-energy-site-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-site-info-api-openapi.yml
- filename: tesla-energy-storm-mode-api-openapi.yml
  format: yaml
  label: Tesla Energy Storm Mode API
  slug: tesla-energy-storm-mode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-storm-mode-api-openapi.yml
- filename: tesla-energy-time-of-use-api-openapi.yml
  format: yaml
  label: Tesla Energy Time Of Use API
  slug: tesla-energy-time-of-use-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/openapi/tesla-energy-time-of-use-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tesla.com
  spf: true
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: www.tesla.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: developer.tesla.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: fleet-api.prd.na.vn.cloud.tesla.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tesla Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tesla Energy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tesla Energy
provider_slug: tesla-energy
slug: tesla-energy-domain-security
source_filename: tesla-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tesla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\n- host: developer.tesla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: fleet-api.prd.na.vn.cloud.tesla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tesla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesla-energy/refs/heads/main/security/tesla-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Clean Energy
- Solar
- Battery Storage
- Powerwall
- Megapack
- Solar Roof
- Virtual Power Plant
- IoT
- Grid Services
- Home Energy
- Utility Scale
---
