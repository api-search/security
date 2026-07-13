---
api_key_in: []
api_specs:
- filename: surveymonkey-openapi.yml
  format: yaml
  label: SurveyMonkey API v3
  slug: rest-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surveymonkey/refs/heads/main/openapi/surveymonkey-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Surveymonkey Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: SurveyMonkey secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: SurveyMonkey
provider_slug: surveymonkey
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.surveymonkey.com/oauth/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://api.surveymonkey.com/oauth/token
  name: oauth2
  sources:
  - openapi/surveymonkey-openapi.yml
  type: oauth2
slug: surveymonkey-authentication
source_filename: surveymonkey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/surveymonkey-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.surveymonkey.com/oauth/authorize\n    tokenUrl: https://api.surveymonkey.com/oauth/token\n    scopes: 7\n  sources:\n  - openapi/surveymonkey-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surveymonkey/refs/heads/main/authentication/surveymonkey-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Surveys
- Market Research
- Feedback
- NPS
- Forms
- OAuth
---
