---
api_key_in: []
api_specs:
- filename: agricultural-marketing-service-mars-api.yaml
  format: yaml
  label: USDA AMS MARS API (MyMarketNews)
  slug: usda-ams-mars-api-mymarketnews
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/openapi/agricultural-marketing-service-mars-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Agricultural Marketing Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agricultural Marketing Service secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agricultural Marketing Service
provider_slug: agricultural-marketing-service
scheme_count: 1
schemes:
- description: API key obtained from USDA AMS MyMarketNews registration. Use the API key as the username with an empty password, or encode as Base64 for Bearer auth. Public access without authentication is also available with lower rate limits.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/agricultural-marketing-service-mars-api.yaml
  type: http
slug: agricultural-marketing-service-authentication
source_filename: agricultural-marketing-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agricultural-marketing-service-mars-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: API key obtained from USDA AMS MyMarketNews registration. Use the API key as\n    the username with an empty password, or encode as Base64 for Bearer auth. Public access\n    without authentication is also available with lower rate limits.\n  sources:\n  - openapi/agricultural-marketing-service-mars-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/authentication/agricultural-marketing-service-authentication.yml
summary_line: http · 1 scheme
tags:
- Agriculture
- Federal Government
- Market News
- Livestock
- Dairy
- Fruits And Vegetables
- Cotton
- Tobacco
---
