---
api_specs:
- filename: atandt-device-status-api-openapi.yml
  format: yaml
  label: AT&T Device Status API
  slug: atandt-device-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-device-status-api-openapi.yml
- filename: atandt-network-insights-api-openapi.yml
  format: yaml
  label: AT&T Network Insights API
  slug: atandt-network-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-network-insights-api-openapi.yml
- filename: atandt-number-verification-api-openapi.yml
  format: yaml
  label: AT&T Number Verification API
  slug: atandt-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-number-verification-api-openapi.yml
- filename: atandt-order-management-api-openapi.yml
  format: yaml
  label: AT&T Order Management API
  slug: atandt-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-order-management-api-openapi.yml
- filename: atandt-product-ordering-api-openapi.yml
  format: yaml
  label: AT&T Product Ordering API
  slug: atandt-product-ordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-product-ordering-api-openapi.yml
- filename: atandt-quality-on-demand-api-openapi.yml
  format: yaml
  label: AT&T Quality on Demand API
  slug: atandt-quality-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-quality-on-demand-api-openapi.yml
- filename: atandt-service-qualification-api-openapi.yml
  format: yaml
  label: AT&T Service Qualification API
  slug: atandt-service-qualification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-service-qualification-api-openapi.yml
- filename: atandt-sim-swap-api-openapi.yml
  format: yaml
  label: AT&T SIM Swap API
  slug: atandt-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-sim-swap-api-openapi.yml
- filename: atandt-threat-detection-api-openapi.yml
  format: yaml
  label: AT&T Threat Detection API
  slug: atandt-threat-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/openapi/atandt-threat-detection-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: att.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: www.att.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: developer.att.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: api.att.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atandt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AT&T, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AT&T
provider_slug: atandt
slug: atandt-domain-security
source_filename: atandt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.att.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developer.att.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.att.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: att.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/security/atandt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 100
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
---
