---
api_specs:
- filename: alaska-air-airports-api-openapi.yml
  format: yaml
  label: Alaska Airlines Airports API
  slug: alaska-air-airports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-airports-api-openapi.yml
- filename: alaska-air-flight-status-api-openapi.yml
  format: yaml
  label: Alaska Airlines Flight Status API
  slug: alaska-air-flight-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-flight-status-api-openapi.yml
- filename: alaska-air-members-api-openapi.yml
  format: yaml
  label: Alaska Airlines Members API
  slug: alaska-air-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-members-api-openapi.yml
- filename: alaska-air-partner-miles-api-openapi.yml
  format: yaml
  label: Alaska Airlines Partner Miles API
  slug: alaska-air-partner-miles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-partner-miles-api-openapi.yml
- filename: alaska-air-rates-api-openapi.yml
  format: yaml
  label: Alaska Airlines Rates API
  slug: alaska-air-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-rates-api-openapi.yml
- filename: alaska-air-schedules-api-openapi.yml
  format: yaml
  label: Alaska Airlines Schedules API
  slug: alaska-air-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-schedules-api-openapi.yml
- filename: alaska-air-shipments-api-openapi.yml
  format: yaml
  label: Alaska Airlines Shipments API
  slug: alaska-air-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-shipments-api-openapi.yml
- filename: alaska-air-transactions-api-openapi.yml
  format: yaml
  label: Alaska Airlines Transactions API
  slug: alaska-air-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alaskaair.com
  spf: true
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: www.alaskaair.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: developers.alaskaair.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.alaskaair.com
  https: false
kind: domain-security
layout: security
method: probed
name: Alaska Air Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alaska Airlines, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alaska Airlines
provider_slug: alaska-air
slug: alaska-air-domain-security
source_filename: alaska-air-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alaskaair.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developers.alaskaair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.alaskaair.com\n  https: false\ndomains:\n- domain: alaskaair.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/security/alaska-air-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
- Fortune 500
---
