---
api_key_in:
- header
api_specs:
- filename: navistone-api-info-api-openapi.yml
  format: yaml
  label: NaviStone API Info API
  slug: navistone-api-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-api-info-api-openapi.yml
- filename: navistone-campaigns-api-openapi.yml
  format: yaml
  label: NaviStone Campaigns API
  slug: navistone-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-campaigns-api-openapi.yml
- filename: navistone-clients-api-openapi.yml
  format: yaml
  label: NaviStone Clients API
  slug: navistone-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-clients-api-openapi.yml
- filename: navistone-domains-api-openapi.yml
  format: yaml
  label: NaviStone Domains API
  slug: navistone-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-domains-api-openapi.yml
- filename: navistone-geo-targeting-api-openapi.yml
  format: yaml
  label: NaviStone Geo Targeting API
  slug: navistone-geo-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-geo-targeting-api-openapi.yml
- filename: navistone-health-api-openapi.yml
  format: yaml
  label: NaviStone Health API
  slug: navistone-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-health-api-openapi.yml
- filename: navistone-output-api-openapi.yml
  format: yaml
  label: NaviStone Output API
  slug: navistone-output-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-output-api-openapi.yml
- filename: navistone-segments-api-openapi.yml
  format: yaml
  label: NaviStone Segments API
  slug: navistone-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-segments-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Navistone Authentication
name_suffix: Authentication
oauth_flows: []
overview: NaviStone secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NaviStone
provider_slug: navistone
scheme_count: 1
schemes:
- description: API Key for authentication
  in: header
  name: api-key
  parameter: X-API-Key
  sources:
  - openapi/navistone-api-info-api-openapi.yml
  - openapi/navistone-campaigns-api-openapi.yml
  - openapi/navistone-clients-api-openapi.yml
  - openapi/navistone-domains-api-openapi.yml
  - openapi/navistone-geo-targeting-api-openapi.yml
  - openapi/navistone-health-api-openapi.yml
  - openapi/navistone-output-api-openapi.yml
  - openapi/navistone-segments-api-openapi.yml
  type: apiKey
slug: navistone-authentication
source_filename: navistone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/navistone-api-info-api-openapi.yml, openapi/navistone-campaigns-api-openapi.yml,\n  openapi/navistone-clients-api-openapi.yml, openapi/navistone-domains-api-openapi.yml, openapi/navistone-geo-targeting-api-openapi.yml,\n  openapi/navistone-health-api-openapi.yml, openapi/navistone-output-api-openapi.yml, openapi/navistone-segments-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API Key for authentication\n  sources:\n  - openapi/navistone-api-info-api-openapi.yml\n  - openapi/navistone-campaigns-api-openapi.yml\n  - openapi/navistone-clients-api-openapi.yml\n  - openapi/navistone-domains-api-openapi.yml\n  - openapi/navistone-geo-targeting-api-openapi.yml\n  - openapi/navistone-health-api-openapi.yml\n  - openapi/navistone-output-api-openapi.yml\n  - openapi/navistone-segments-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/authentication/navistone-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Marketing
- Direct Mail
- Advertising
- Customer Acquisition
- Audience Targeting
- MarTech
- AdTech
- Postcards
- Retargeting
---
