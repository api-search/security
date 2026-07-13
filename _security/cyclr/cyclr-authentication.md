---
api_key_in: []
api_specs:
- filename: cyclr-cyclr-openapi.yml
  format: yaml
  label: Cyclr API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/openapi/cyclr-cyclr-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cyclr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cyclr secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cyclr
provider_slug: cyclr
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token obtained from the /oauth/token endpoint using Client Credentials flow with your Cyclr Console Client ID and Client Secret.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cyclr-cyclr-openapi.yml
  type: http
slug: cyclr-authentication
source_filename: cyclr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cyclr-cyclr-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token obtained from the /oauth/token endpoint using Client Credentials\n    flow with your Cyclr Console Client ID and Client Secret.\n  sources:\n  - openapi/cyclr-cyclr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyclr/refs/heads/main/authentication/cyclr-authentication.yml
summary_line: http · 1 scheme
tags:
- Connectors
- Custom Connectors
- Data Synchronization
- Embedded iPaaS
- Embedded SaaS Integration
- Embedded UI
- Integration Platform
- Integrations
- Marketplace
- OAuth 2.0
- REST API
- SaaS
- Templates
- Webhooks
- White Label
- Workflows
---
