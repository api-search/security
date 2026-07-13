---
api_key_in: []
api_specs:
- filename: allianz-engagement-survey.yaml
  format: yaml
  label: Allianz Engagement Survey API
  slug: engagement-survey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/openapi/allianz-engagement-survey.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Allianz Engagement Survey Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Allianz Engagement Survey secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
scheme_count: 1
schemes:
- description: OAuth2 client credentials for Allianz internal API access
  flows:
  - flow: clientCredentials
    scopes: 5
    tokenUrl: https://api.allianz.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/allianz-engagement-survey.yaml
  type: oauth2
slug: allianz-engagement-survey-authentication
source_filename: allianz-engagement-survey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/allianz-engagement-survey.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.allianz.com/oauth2/token\n    scopes: 5\n  description: OAuth2 client credentials for Allianz internal API access\n  sources:\n  - openapi/allianz-engagement-survey.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/authentication/allianz-engagement-survey-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
---
