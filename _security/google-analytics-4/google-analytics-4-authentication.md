---
api_key_in: []
api_specs:
- filename: rest
  format: yaml
  label: Google Analytics Data API
  slug: google-analytics-data-api
  spec_type: OpenAPI
  url: https://analyticsdata.googleapis.com/$discovery/rest?version=v1beta
- filename: rest
  format: yaml
  label: Google Analytics Admin API
  slug: google-analytics-admin-api
  spec_type: OpenAPI
  url: https://analyticsadmin.googleapis.com/$discovery/rest?version=v1beta
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Analytics 4 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Analytics 4 secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Analytics 4
provider_slug: google-analytics-4
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-analytics-4-openapi.yml
  type: oauth2
slug: google-analytics-4-authentication
source_filename: google-analytics-4-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-analytics-4-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/google-analytics-4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/authentication/google-analytics-4-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Data Collection
- Marketing
- Measurement
- Mobile Analytics
- Reporting
- Web Analytics
---
