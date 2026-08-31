---
api_specs:
- filename: spp-forecasting-api-openapi.yml
  format: yaml
  label: Southwest Power Pool Forecasting API
  slug: spp-forecasting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/openapi/spp-forecasting-api-openapi.yml
- filename: spp-monitoring-sets-api-openapi.yml
  format: yaml
  label: Southwest Power Pool Monitoring Sets API
  slug: spp-monitoring-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/openapi/spp-monitoring-sets-api-openapi.yml
- filename: spp-real-time-api-openapi.yml
  format: yaml
  label: Southwest Power Pool Real Time API
  slug: spp-real-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/openapi/spp-real-time-api-openapi.yml
- filename: spp-seasonal-api-openapi.yml
  format: yaml
  label: Southwest Power Pool Seasonal API
  slug: spp-seasonal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/openapi/spp-seasonal-api-openapi.yml
- filename: spp-seasonal-overrides-api-openapi.yml
  format: yaml
  label: Southwest Power Pool Seasonal Overrides API
  slug: spp-seasonal-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/openapi/spp-seasonal-overrides-api-openapi.yml
- filename: spp-temporary-aar-exceptions-api-openapi.yml
  format: yaml
  label: Southwest Power Pool Temporary AAR Exceptions API
  slug: spp-temporary-aar-exceptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/openapi/spp-temporary-aar-exceptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spp.org
  spf: true
hosts:
- cert_expires: Jan 29 18:24:24 2027 GMT
  host: www.spp.org
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  9 13:43:12 2027 GMT
  host: portal.spp.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 29 18:24:24 2027 GMT
  host: spp.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Spp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Southwest Power Pool, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Southwest Power Pool
provider_slug: spp
slug: spp-domain-security
source_filename: spp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spp.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 18:24:24 2027 GMT\n  hsts: false\n- host: portal.spp.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  9 13:43:12 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: spp.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 18:24:24 2027 GMT\n  hsts: false\ndomains:\n- domain: spp.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/security/spp-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Energy
- United States
- Energy Markets
- Electricity
- Grid
- Utilities
- Renewables
- Market Data
- Transmission
- System Operator
---
