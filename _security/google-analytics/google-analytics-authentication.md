---
api_key_in: []
api_specs:
- filename: google-analytics-data-api.yaml
  format: yaml
  label: Google Analytics Data API (GA4)
  slug: google-analytics-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-data-api.yaml
- filename: google-analytics-admin-api.yaml
  format: yaml
  label: Google Analytics Admin API
  slug: google-analytics-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-admin-api.yaml
- filename: google-analytics-measurement-protocol.yaml
  format: yaml
  label: Google Analytics Measurement Protocol (GA4)
  slug: google-analytics-measurement-protocol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-measurement-protocol.yaml
- filename: google-analytics-user-deletion-api.yaml
  format: yaml
  label: Google Analytics User Deletion API
  slug: google-analytics-user-deletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-user-deletion-api.yaml
- filename: google-analytics-reporting-api-v4.yaml
  format: yaml
  label: Google Analytics Reporting API v4 (Universal Analytics)
  slug: google-analytics-reporting-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-reporting-api-v4.yaml
- filename: google-analytics-management-api-v3.yaml
  format: yaml
  label: Google Analytics Management API v3
  slug: google-analytics-management-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-management-api-v3.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Analytics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Google Analytics secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Google Analytics
provider_slug: google-analytics
scheme_count: 2
schemes:
- description: Oauth 2.0 implicit authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: implicit
    scopes: 2
  name: Oauth2
  sources:
  - openapi/google-analytics-admin-api.yaml
  - openapi/google-analytics-data-api.yaml
  - openapi/google-analytics-management-api-v3.yaml
  - openapi/google-analytics-reporting-api-v4.yaml
  type: oauth2
- description: Oauth 2.0 authorizationCode authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://accounts.google.com/o/oauth2/token
  name: Oauth2c
  sources:
  - openapi/google-analytics-admin-api.yaml
  - openapi/google-analytics-data-api.yaml
  - openapi/google-analytics-management-api-v3.yaml
  - openapi/google-analytics-reporting-api-v4.yaml
  - openapi/google-analytics-user-deletion-api.yaml
  type: oauth2
slug: google-analytics-authentication
source_filename: google-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-analytics-admin-api.yaml, openapi/google-analytics-data-api.yaml, openapi/google-analytics-management-api-v3.yaml,\n  openapi/google-analytics-reporting-api-v4.yaml, openapi/google-analytics-user-deletion-api.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: Oauth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    scopes: 2\n  description: Oauth 2.0 implicit authentication\n  sources:\n  - openapi/google-analytics-admin-api.yaml\n  - openapi/google-analytics-data-api.yaml\n  - openapi/google-analytics-management-api-v3.yaml\n  - openapi/google-analytics-reporting-api-v4.yaml\n- name: Oauth2c\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://accounts.google.com/o/oauth2/token\n    scopes: 2\n  description:\
  \ Oauth 2.0 authorizationCode authentication\n  sources:\n  - openapi/google-analytics-admin-api.yaml\n  - openapi/google-analytics-data-api.yaml\n  - openapi/google-analytics-management-api-v3.yaml\n  - openapi/google-analytics-reporting-api-v4.yaml\n  - openapi/google-analytics-user-deletion-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/authentication/google-analytics-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
---
