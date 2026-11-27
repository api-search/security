---
anonymous_access: false
api_key_in: []
api_specs:
- filename: meridary-com-agent-api-openapi.yml
  format: yaml
  label: Meridary Agent API
  slug: meridary-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meridary-com/openapi/meridary-com-agent-api-openapi.yml
- filename: meridary-com-calculators-api-openapi.yml
  format: yaml
  label: Meridary Calculators API
  slug: meridary-com-calculators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meridary-com/openapi/meridary-com-calculators-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Meridary Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Meridary secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Meridary
provider_slug: meridary-com
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://www.meridary.com/api/auth/oauth2/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://www.meridary.com/api/auth/oauth2/token
  name: agentOAuth
  sources:
  - openapi/meridary-com-openapi.yml
  type: oauth2
slug: meridary-com-authentication
source_filename: meridary-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/meridary-com-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: agentOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.meridary.com/api/auth/oauth2/authorize\n    tokenUrl: https://www.meridary.com/api/auth/oauth2/token\n    scopes: 7\n  sources:\n  - openapi/meridary-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/meridary-com/authentication/meridary-com-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Finance
- Retirement
- Planning
- Calculator
- Software-as-a-Service
---
