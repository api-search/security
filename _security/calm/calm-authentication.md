---
api_key_in: []
api_specs:
- filename: calm-partner-api-openapi.yml
  format: yaml
  label: Calm Partner API
  slug: calm-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calm/refs/heads/main/openapi/calm-partner-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Calm Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Calm secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Calm
provider_slug: calm
scheme_count: 1
schemes:
- description: OAuth 2.0 client-credentials grant against the Calm auth service.
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://auth.calm.com/v0/authorize
  name: CalmOAuth2
  sources:
  - openapi/calm-partner-api-openapi.yml
  type: oauth2
slug: calm-authentication
source_filename: calm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/calm-partner-api-openapi.yml\ndocs: https://partner.calm.com/docs/api\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: CalmOAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.calm.com/v0/authorize\n    scopes: 2\n  description: OAuth 2.0 client-credentials grant against the Calm auth service.\n  sources:\n  - openapi/calm-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calm/refs/heads/main/authentication/calm-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Mental Health
- Wellness
- Meditation
- Mindfulness
- Sleep
- Employee Benefits
- Health
- B2B
- Subscriptions
---
