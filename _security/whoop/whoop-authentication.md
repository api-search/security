---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: WHOOP API
  slug: whoop-api
  spec_type: OpenAPI
  url: https://developer.whoop.com/api/
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Whoop Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: WHOOP secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: WHOOP
provider_slug: whoop
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://api.prod.whoop.com/oauth/oauth2/auth
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://api.prod.whoop.com/oauth/oauth2/token
  name: OAuth
  sources:
  - openapi/whoop-openapi.yml
  type: oauth2
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.prod.whoop.com/developer/v2/partner/token
  name: Trusted Partner
  sources:
  - openapi/whoop-openapi.yml
  type: oauth2
slug: whoop-authentication
source_filename: whoop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/whoop-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.prod.whoop.com/oauth/oauth2/auth\n    tokenUrl: https://api.prod.whoop.com/oauth/oauth2/token\n    scopes: 6\n  sources:\n  - openapi/whoop-openapi.yml\n- name: Trusted Partner\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.prod.whoop.com/developer/v2/partner/token\n    scopes: 1\n  sources:\n  - openapi/whoop-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whoop/refs/heads/main/authentication/whoop-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Fitness
- Wearables
- Health
- Recovery
- Sleep
- Workout
- Strain
- Heart Rate
- Performance
---
