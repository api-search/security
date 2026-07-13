---
api_key_in: []
api_specs:
- filename: google-campaign-manager-openapi.yml
  format: yaml
  label: Campaign Manager 360 API
  slug: campaign-manager-360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/openapi/google-campaign-manager-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Campaign Manager Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Campaign Manager secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication for accessing Campaign Manager 360 resources. Requires appropriate scopes for trafficking or reporting operations.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-campaign-manager-openapi.yml
  type: oauth2
slug: google-campaign-manager-authentication
source_filename: google-campaign-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-campaign-manager-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  description: OAuth 2.0 authentication for accessing Campaign Manager 360 resources. Requires\n    appropriate scopes for trafficking or reporting operations.\n  sources:\n  - openapi/google-campaign-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/authentication/google-campaign-manager-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
---
