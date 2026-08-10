---
api_specs:
- filename: climateai-platform-swagger.json
  format: json
  label: ClimateAI Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/_original/climateai-platform-swagger.json
- filename: climateai-account-api-openapi.yml
  format: yaml
  label: ClimateAI Account API
  slug: climateai-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-account-api-openapi.yml
- filename: climateai-account-config-api-openapi.yml
  format: yaml
  label: ClimateAI Account Config API
  slug: climateai-account-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-account-config-api-openapi.yml
- filename: climateai-auth-api-openapi.yml
  format: yaml
  label: ClimateAI Auth API
  slug: climateai-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-auth-api-openapi.yml
- filename: climateai-current-v2-api-openapi.yml
  format: yaml
  label: ClimateAI Current (v2) API
  slug: climateai-current-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-current-v2-api-openapi.yml
- filename: climateai-device-api-openapi.yml
  format: yaml
  label: ClimateAI Device API
  slug: climateai-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-device-api-openapi.yml
- filename: climateai-email-api-openapi.yml
  format: yaml
  label: ClimateAI Email API
  slug: climateai-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-email-api-openapi.yml
- filename: climateai-legacy-v1-api-openapi.yml
  format: yaml
  label: ClimateAI Legacy (v1) API
  slug: climateai-legacy-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-legacy-v1-api-openapi.yml
- filename: climateai-permission-api-openapi.yml
  format: yaml
  label: ClimateAI Permission API
  slug: climateai-permission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-permission-api-openapi.yml
- filename: climateai-platform-api-openapi.yml
  format: yaml
  label: ClimateAI Platform API
  slug: climateai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-platform-api-openapi.yml
- filename: climateai-product-api-openapi.yml
  format: yaml
  label: ClimateAI Product API
  slug: climateai-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-product-api-openapi.yml
- filename: climateai-report-api-openapi.yml
  format: yaml
  label: ClimateAI Report API
  slug: climateai-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-report-api-openapi.yml
- filename: climateai-role-api-openapi.yml
  format: yaml
  label: ClimateAI Role API
  slug: climateai-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-role-api-openapi.yml
- filename: climateai-routing-api-openapi.yml
  format: yaml
  label: ClimateAI Routing API
  slug: climateai-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-routing-api-openapi.yml
- filename: climateai-user-api-openapi.yml
  format: yaml
  label: ClimateAI User API
  slug: climateai-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/openapi/climateai-user-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: climate.ai
  spf: true
hosts:
- cert_expires: Sep 27 15:41:04 2026 GMT
  host: climate.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 13:39:01 2026 GMT
  host: docs.climate.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api-prod.climate.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Climateai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClimateAI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ClimateAI
provider_slug: climateai
slug: climateai-domain-security
source_filename: climateai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: climate.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:41:04 2026 GMT\n  hsts: null\n- host: docs.climate.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 13:39:01 2026 GMT\n  hsts: null\n- host: api-prod.climate.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: climate.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climateai/refs/heads/main/security/climateai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Weather
- Climate
- Climate Intelligence
- Forecasting
- Agriculture
- Data
- Supply Chain
- Risk
- Sustainability
---
