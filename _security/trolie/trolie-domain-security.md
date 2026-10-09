---
api_specs:
- filename: trolie-forecasting-api-openapi.yml
  format: yaml
  label: TROLIE Forecasting API
  slug: trolie-forecasting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-forecasting-api-openapi.yml
- filename: trolie-monitoring-sets-api-openapi.yml
  format: yaml
  label: TROLIE Monitoring Sets API
  slug: trolie-monitoring-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-monitoring-sets-api-openapi.yml
- filename: trolie-seasonal-api-openapi.yml
  format: yaml
  label: TROLIE Seasonal API
  slug: trolie-seasonal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-seasonal-api-openapi.yml
- filename: trolie-seasonal-overrides-api-openapi.yml
  format: yaml
  label: TROLIE Seasonal Overrides API
  slug: trolie-seasonal-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-seasonal-overrides-api-openapi.yml
- filename: trolie-temporary-aar-exceptions-api-openapi.yml
  format: yaml
  label: TROLIE Temporary AAR Exceptions API
  slug: trolie-temporary-aar-exceptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-temporary-aar-exceptions-api-openapi.yml
- filename: trolie-realtime-api-openapi.yml
  format: yaml
  label: TROLIE Realtime API
  slug: trolie-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-realtime-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trolie.energy
  spf: false
hosts:
- cert_expires: Nov 28 18:38:21 2026 GMT
  host: trolie.energy
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trolie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TROLIE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TROLIE
provider_slug: trolie
slug: trolie-domain-security
source_filename: trolie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trolie.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 18:38:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: trolie.energy\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/security/trolie-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Energy
- Electric Grid
- Transmission
- Open Standards
- OpenAPI
- LF Energy
- Open Source
---
