---
api_key_in: []
api_specs:
- filename: project44-shipments-api-openapi.yml
  format: yaml
  label: project44 Shipments API
  slug: project44-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/project44/refs/heads/main/openapi/project44-shipments-api-openapi.yml
- filename: project44-status-api-openapi.yml
  format: yaml
  label: project44 Status API
  slug: project44-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/project44/refs/heads/main/openapi/project44-status-api-openapi.yml
- filename: project44-tracking-api-openapi.yml
  format: yaml
  label: project44 Tracking API
  slug: project44-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/project44/refs/heads/main/openapi/project44-tracking-api-openapi.yml
- filename: project44-webhooks-api-openapi.yml
  format: yaml
  label: project44 Webhooks API
  slug: project44-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/project44/refs/heads/main/openapi/project44-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Project44 Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: project44 secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: project44
provider_slug: project44
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://api.project44.com/api/v4/oauth2/token
  name: oauth2
  sources:
  - openapi/project44-tracking-openapi.yml
  type: oauth2
slug: project44-authentication
source_filename: project44-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/project44-tracking-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.project44.com/api/v4/oauth2/token\n    scopes: 3\n  sources:\n  - openapi/project44-tracking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/project44/refs/heads/main/authentication/project44-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Logistics
- Supply Chain Visibility
- Tracking
- Freight
- Multi-Modal
---
