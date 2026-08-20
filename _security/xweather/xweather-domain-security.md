---
api_specs:
- filename: xweather-air-quality-api-openapi.yml
  format: yaml
  label: Xweather Air Quality API
  slug: xweather-air-quality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xweather/refs/heads/main/openapi/xweather-air-quality-api-openapi.yml
- filename: xweather-alerts-api-openapi.yml
  format: yaml
  label: Xweather Alerts API
  slug: xweather-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xweather/refs/heads/main/openapi/xweather-alerts-api-openapi.yml
- filename: xweather-conditions-api-openapi.yml
  format: yaml
  label: Xweather Conditions API
  slug: xweather-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xweather/refs/heads/main/openapi/xweather-conditions-api-openapi.yml
- filename: xweather-fires-api-openapi.yml
  format: yaml
  label: Xweather Fires API
  slug: xweather-fires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xweather/refs/heads/main/openapi/xweather-fires-api-openapi.yml
- filename: xweather-forecasts-api-openapi.yml
  format: yaml
  label: Xweather Forecasts API
  slug: xweather-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xweather/refs/heads/main/openapi/xweather-forecasts-api-openapi.yml
- filename: xweather-lightning-api-openapi.yml
  format: yaml
  label: Xweather Lightning API
  slug: xweather-lightning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xweather/refs/heads/main/openapi/xweather-lightning-api-openapi.yml
- filename: xweather-maritime-api-openapi.yml
  format: yaml
  label: Xweather Maritime API
  slug: xweather-maritime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xweather/refs/heads/main/openapi/xweather-maritime-api-openapi.yml
- filename: xweather-observations-api-openapi.yml
  format: yaml
  label: Xweather Observations API
  slug: xweather-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xweather/refs/heads/main/openapi/xweather-observations-api-openapi.yml
- filename: xweather-tropical-api-openapi.yml
  format: yaml
  label: Xweather Tropical API
  slug: xweather-tropical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xweather/refs/heads/main/openapi/xweather-tropical-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xweather.com
  spf: true
hosts:
- cert_expires: Sep 21 07:19:01 2026 GMT
  host: xweather.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 07:39:58 2026 GMT
  host: www.xweather.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: data.api.xweather.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xweather Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xweather, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Xweather
provider_slug: xweather
slug: xweather-domain-security
source_filename: xweather-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xweather.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:19:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.xweather.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 07:39:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: data.api.xweather.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: xweather.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xweather/refs/heads/main/security/xweather-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Air Quality
- Company
- Data
- Forecast
- Lightning
- Maritime
- Observations
- Severe Weather
- Weather
---
