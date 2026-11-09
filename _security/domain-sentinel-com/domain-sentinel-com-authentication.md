---
anonymous_access: false
api_key_in: []
api_specs:
- filename: domain-sentinel-com-lookup-api-openapi.yml
  format: yaml
  label: Domain Sentinel Lookup API
  slug: domain-sentinel-com-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domain-sentinel-com/openapi/domain-sentinel-com-lookup-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Domain Sentinel Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Domain Sentinel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Domain Sentinel
provider_slug: domain-sentinel-com
scheme_count: 1
schemes:
- description: API key created in the dashboard (ds_live_...)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/domain-sentinel-com-openapi.yml
  type: http
slug: domain-sentinel-com-authentication
source_filename: domain-sentinel-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/domain-sentinel-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key created in the dashboard (ds_live_...)\n  sources:\n  - openapi/domain-sentinel-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/domain-sentinel-com/authentication/domain-sentinel-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Domain Monitoring
- WHOIS Lookup
- RDAP API
- Brand Protection
- Expiry Alerts
- DNS Monitoring
---
