---
api_key_in:
- header
api_specs:
- filename: unmade-embed-v2-openapi.json
  format: json
  label: Unmade Integration API (V2)
  slug: unmade-integration-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unmade/refs/heads/main/openapi/unmade-embed-v2-openapi.json
- filename: unmade-embed-v1-openapi.json
  format: json
  label: Unmade Integration API (V1)
  slug: unmade-integration-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unmade/refs/heads/main/openapi/unmade-embed-v1-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Unmade Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unmade secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unmade
provider_slug: unmade
scheme_count: 1
schemes:
- description: 'Token authentication. Unmade provides your unique token; send it as `Authorization: Token <token>`. All API URLs are partner-specific subdomains and every endpoint URL must end with a trailing slash.'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/unmade-embed-v1-openapi.json
  - openapi/unmade-embed-v2-openapi.json
  type: apiKey
slug: unmade-authentication
source_filename: unmade-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/unmade-embed-v1-openapi.json, openapi/unmade-embed-v2-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Token authentication. Unmade provides your unique token; send it as `Authorization:\n    Token <token>`. All API URLs are partner-specific subdomains and every endpoint URL must\n    end with a trailing slash.'\n  sources:\n  - openapi/unmade-embed-v1-openapi.json\n  - openapi/unmade-embed-v2-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unmade/refs/heads/main/authentication/unmade-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fashion
- Apparel
- Manufacturing
- Customization
- eCommerce
- On-Demand Production
- Embedded Commerce
---
