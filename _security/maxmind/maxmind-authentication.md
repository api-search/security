---
api_key_in: []
api_specs:
- filename: maxmind-geoip-openapi.yml
  format: yaml
  label: GeoIP Country Web Service
  slug: geoip-country
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-geoip-openapi.yml
- filename: maxmind-geoip-openapi.yml
  format: yaml
  label: GeoIP City Plus Web Service
  slug: geoip-city
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-geoip-openapi.yml
- filename: maxmind-geoip-openapi.yml
  format: yaml
  label: GeoIP Insights Web Service
  slug: geoip-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-geoip-openapi.yml
- filename: maxmind-minfraud-openapi.yml
  format: yaml
  label: minFraud Score
  slug: minfraud-score
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-minfraud-openapi.yml
- filename: maxmind-minfraud-openapi.yml
  format: yaml
  label: minFraud Insights
  slug: minfraud-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-minfraud-openapi.yml
- filename: maxmind-minfraud-openapi.yml
  format: yaml
  label: minFraud Factors
  slug: minfraud-factors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/openapi/maxmind-minfraud-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Maxmind Authentication
name_suffix: Authentication
oauth_flows: []
overview: MaxMind secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MaxMind
provider_slug: maxmind
scheme_count: 1
schemes:
- description: Use your MaxMind account ID as the username and your license key as the password. All requests must be made over HTTPS.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/maxmind-geoip-openapi.yml
  - openapi/maxmind-minfraud-openapi.yml
  type: http
slug: maxmind-authentication
source_filename: maxmind-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/maxmind-geoip-openapi.yml, openapi/maxmind-minfraud-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Use your MaxMind account ID as the username and your license key as the password.\n    All requests must be made over HTTPS.\n  sources:\n  - openapi/maxmind-geoip-openapi.yml\n  - openapi/maxmind-minfraud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maxmind/refs/heads/main/authentication/maxmind-authentication.yml
summary_line: http · 1 scheme
tags:
- IP Intelligence
- Geolocation
- Fraud Prevention
- Risk Scoring
- VPN Detection
- Proxy Detection
- ISP Data
- GeoIP
---
