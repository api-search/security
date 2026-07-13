---
api_key_in:
- header
api_specs:
- filename: smartrecruiters-posting-openapi.yml
  format: yaml
  label: SmartRecruiters Posting API
  slug: posting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrecruiters/refs/heads/main/openapi/smartrecruiters-posting-openapi.yml
- filename: smartrecruiters-jobs-openapi.yml
  format: yaml
  label: SmartRecruiters Job API
  slug: job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrecruiters/refs/heads/main/openapi/smartrecruiters-jobs-openapi.yml
- filename: smartrecruiters-candidates-openapi.yml
  format: yaml
  label: SmartRecruiters Candidate API
  slug: candidate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartrecruiters/refs/heads/main/openapi/smartrecruiters-candidates-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Smartrecruiters Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: SmartRecruiters secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: SmartRecruiters
provider_slug: smartrecruiters
scheme_count: 3
schemes:
- in: header
  name: ApiKey
  parameter: X-SmartToken
  sources:
  - openapi/smartrecruiters-candidates-openapi.yml
  - openapi/smartrecruiters-jobs-openapi.yml
  - openapi/smartrecruiters-posting-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://www.smartrecruiters.com/identity/oauth/token
  name: OAuth2
  sources:
  - openapi/smartrecruiters-candidates-openapi.yml
  - openapi/smartrecruiters-jobs-openapi.yml
  type: oauth2
- flows:
  - authorizationUrl: https://www.smartrecruiters.com/identity/oauth/allow
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://www.smartrecruiters.com/identity/oauth/token
  name: OAuth2
  sources:
  - openapi/smartrecruiters-posting-openapi.yml
  type: oauth2
slug: smartrecruiters-authentication
source_filename: smartrecruiters-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smartrecruiters-candidates-openapi.yml, openapi/smartrecruiters-jobs-openapi.yml,\n  openapi/smartrecruiters-posting-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-SmartToken\n  sources:\n  - openapi/smartrecruiters-candidates-openapi.yml\n  - openapi/smartrecruiters-jobs-openapi.yml\n  - openapi/smartrecruiters-posting-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.smartrecruiters.com/identity/oauth/token\n    scopes: 2\n  sources:\n  - openapi/smartrecruiters-candidates-openapi.yml\n  - openapi/smartrecruiters-jobs-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.smartrecruiters.com/identity/oauth/allow\n    tokenUrl:\
  \ https://www.smartrecruiters.com/identity/oauth/token\n    scopes: 4\n  sources:\n  - openapi/smartrecruiters-posting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartrecruiters/refs/heads/main/authentication/smartrecruiters-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Human Resources
- Recruiting
- Talent Acquisition
- Applicant Tracking
- HR Technology
---
