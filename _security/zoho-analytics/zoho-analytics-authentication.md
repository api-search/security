---
api_key_in: []
api_specs:
- filename: analytics-oas
  format: yaml
  label: Zoho Analytics API
  slug: zoho-analytics-api
  spec_type: OpenAPI
  url: https://github.com/zoho/analytics-oas
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zoho Analytics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zoho Analytics secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zoho Analytics
provider_slug: zoho-analytics
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: iam-oauth2-schema
  sources:
  - openapi/bulk-api.json
  - openapi/data-api.json
  - openapi/embed-api.json
  - openapi/metadata-api.json
  - openapi/modeling-api.json
  - openapi/share-api.json
  - openapi/usermanagement-api.json
  type: oauth2
slug: zoho-analytics-authentication
source_filename: zoho-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bulk-api.json, openapi/data-api.json, openapi/embed-api.json, openapi/metadata-api.json,\n  openapi/modeling-api.json, openapi/share-api.json, openapi/usermanagement-api.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: iam-oauth2-schema\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n    scopes: 6\n  sources:\n  - openapi/bulk-api.json\n  - openapi/data-api.json\n  - openapi/embed-api.json\n  - openapi/metadata-api.json\n  - openapi/modeling-api.json\n  - openapi/share-api.json\n  - openapi/usermanagement-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-analytics/refs/heads/main/authentication/zoho-analytics-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Business Intelligence
- Analytics
- Dashboards
- Reports
- Data Import
- Data Export
- Workspaces
- Visualizations
---
