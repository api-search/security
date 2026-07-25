---
api_specs:
- filename: powernaut-authentication-api-openapi.yml
  format: yaml
  label: Powernaut authentication API
  slug: powernaut-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-authentication-api-openapi.yml
- filename: powernaut-baselining-api-openapi.yml
  format: yaml
  label: Powernaut baselining API
  slug: powernaut-baselining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-baselining-api-openapi.yml
- filename: powernaut-creating-bids-api-openapi.yml
  format: yaml
  label: Powernaut creating_bids API
  slug: powernaut-creating-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-creating-bids-api-openapi.yml
- filename: powernaut-events-api-openapi.yml
  format: yaml
  label: Powernaut events API
  slug: powernaut-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-events-api-openapi.yml
- filename: powernaut-getting-forecasts-api-openapi.yml
  format: yaml
  label: Powernaut getting_forecasts API
  slug: powernaut-getting-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-getting-forecasts-api-openapi.yml
- filename: powernaut-historical-data-api-openapi.yml
  format: yaml
  label: Powernaut historical_data API
  slug: powernaut-historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-historical-data-api-openapi.yml
- filename: powernaut-managing-bids-api-openapi.yml
  format: yaml
  label: Powernaut managing_bids API
  slug: powernaut-managing-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-managing-bids-api-openapi.yml
- filename: powernaut-markets-api-openapi.yml
  format: yaml
  label: Powernaut markets API
  slug: powernaut-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-markets-api-openapi.yml
- filename: powernaut-metrics-api-openapi.yml
  format: yaml
  label: Powernaut metrics API
  slug: powernaut-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-metrics-api-openapi.yml
- filename: powernaut-resources-api-openapi.yml
  format: yaml
  label: Powernaut resources API
  slug: powernaut-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-resources-api-openapi.yml
- filename: powernaut-sensor-data-api-openapi.yml
  format: yaml
  label: Powernaut sensor_data API
  slug: powernaut-sensor-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-sensor-data-api-openapi.yml
- filename: powernaut-sites-api-openapi.yml
  format: yaml
  label: Powernaut sites API
  slug: powernaut-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-sites-api-openapi.yml
- filename: powernaut-uploading-forecasts-api-openapi.yml
  format: yaml
  label: Powernaut uploading_forecasts API
  slug: powernaut-uploading-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/openapi/powernaut-uploading-forecasts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: powernaut.io
  spf: true
hosts:
- cert_expires: Aug 29 16:11:24 2026 GMT
  host: powernaut.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Powernaut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Powernaut, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Powernaut
provider_slug: powernaut
slug: powernaut-domain-security
source_filename: powernaut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: powernaut.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 16:11:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: powernaut.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powernaut/refs/heads/main/security/powernaut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Virtual Power Plant
- Distributed Energy Resources
- Energy Trading
- Flexibility
- Forecasting
- Grid
---
