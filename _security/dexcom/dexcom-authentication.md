---
api_key_in: []
api_specs:
- filename: dexcom-dexcom-api.yml
  format: yaml
  label: Dexcom Developer API
  slug: dexcom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcom/refs/heads/main/openapi/dexcom-dexcom-api.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Dexcom Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Dexcom secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Dexcom
provider_slug: dexcom
scheme_count: 1
schemes:
- description: Dexcom uses OAuth 2.0 authorization code flow. The only acceptable scope value is `offline_access`.
  flows:
  - authorizationUrl: https://api.dexcom.com/v2/oauth2/login
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.dexcom.com/v2/oauth2/token
  name: OAuth2
  sources:
  - openapi/dexcom-dexcom-api.yml
  type: oauth2
slug: dexcom-authentication
source_filename: dexcom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dexcom-dexcom-api.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.dexcom.com/v2/oauth2/login\n    tokenUrl: https://api.dexcom.com/v2/oauth2/token\n    scopes: 1\n  description: Dexcom uses OAuth 2.0 authorization code flow. The only acceptable scope value\n    is `offline_access`.\n  sources:\n  - openapi/dexcom-dexcom-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dexcom/refs/heads/main/authentication/dexcom-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Continuous Glucose Monitoring
- Diabetes
- Digital Health
- Glucose
- Healthcare
- Medical Devices
- Wearables
---
