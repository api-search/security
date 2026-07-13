---
api_specs:
- filename: alaska-air-flight-status-openapi.yaml
  format: yaml
  label: Alaska Airlines Flight Status API
  slug: flight-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-flight-status-openapi.yaml
- filename: alaska-air-flight-schedules-openapi.yaml
  format: yaml
  label: Alaska Airlines Flight Schedules API
  slug: flight-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-flight-schedules-openapi.yaml
- filename: alaska-air-cargo-openapi.yaml
  format: yaml
  label: Alaska Air Cargo API
  slug: cargo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-cargo-openapi.yaml
- filename: alaska-air-mileage-plan-openapi.yaml
  format: yaml
  label: Alaska Airlines Mileage Plan API
  slug: mileage-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/openapi/alaska-air-mileage-plan-openapi.yaml
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
