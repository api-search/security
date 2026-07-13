---
api_key_in: []
api_specs:
- filename: cms-blue-button-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 Explanation of Benefit API
  slug: cms-blue-button-explanation-of-benefit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/openapi/cms-blue-button-openapi.yml
- filename: cms-blue-button-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 Patient API
  slug: cms-blue-button-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/openapi/cms-blue-button-openapi.yml
- filename: cms-blue-button-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 Coverage API
  slug: cms-blue-button-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/openapi/cms-blue-button-openapi.yml
- filename: cms-blue-button-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 Authorization and UserInfo API
  slug: cms-blue-button-authorization-userinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/openapi/cms-blue-button-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cms Blue Button Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CMS Blue Button 2.0 secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CMS Blue Button 2.0
provider_slug: cms-blue-button
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization-code flow with mandatory PKCE (S256 only). Beneficiaries log in with their Medicare.gov credentials and choose whether to share demographic data. Access tokens expire after 1 hour. One-time-use refresh tokens are issued only to approved 13-month and research application types. Sandbox uses https://sandbox.bluebutton.cms.gov/v2/o/authorize/ and https://sandbox.bluebutton.cms
  flows:
  - authorizationUrl: https://api.bluebutton.cms.gov/v2/o/authorize/
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://api.bluebutton.cms.gov/v2/o/token/
  name: oauth2
  sources:
  - openapi/cms-blue-button-openapi.yml
  type: oauth2
slug: cms-blue-button-authentication
source_filename: cms-blue-button-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cms-blue-button-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.bluebutton.cms.gov/v2/o/authorize/\n    tokenUrl: https://api.bluebutton.cms.gov/v2/o/token/\n    scopes: 6\n  description: OAuth 2.0 authorization-code flow with mandatory PKCE (S256 only). Beneficiaries\n    log in with their Medicare.gov credentials and choose whether to share demographic data.\n    Access tokens expire after 1 hour. One-time-use refresh tokens are issued only to approved\n    13-month and research application types. Sandbox uses https://sandbox.bluebutton.cms.gov/v2/o/authorize/\n    and https://sandbox.bluebutton.cms\n  sources:\n  - openapi/cms-blue-button-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/authentication/cms-blue-button-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Blue Button
- CARIN
- Medicare
- FHIR
- Claims Data
- Patient Access
- Healthcare
- Government
---
