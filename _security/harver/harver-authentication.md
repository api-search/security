---
api_key_in: []
api_specs:
- filename: harver-accounts-api-openapi.yml
  format: yaml
  label: Harver accounts API
  slug: harver-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-accounts-api-openapi.yml
- filename: harver-applications-api-openapi.yml
  format: yaml
  label: Harver applications API
  slug: harver-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-applications-api-openapi.yml
- filename: harver-candidate-statuses-api-openapi.yml
  format: yaml
  label: Harver candidate-statuses API
  slug: harver-candidate-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-candidate-statuses-api-openapi.yml
- filename: harver-candidateapplications-api-openapi.yml
  format: yaml
  label: Harver candidateApplications API
  slug: harver-candidateapplications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-candidateapplications-api-openapi.yml
- filename: harver-oauth-api-openapi.yml
  format: yaml
  label: Harver oauth API
  slug: harver-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-oauth-api-openapi.yml
- filename: harver-scheduling-api-openapi.yml
  format: yaml
  label: Harver scheduling API
  slug: harver-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-scheduling-api-openapi.yml
- filename: harver-user-profile-api-openapi.yml
  format: yaml
  label: Harver user-profile API
  slug: harver-user-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-user-profile-api-openapi.yml
- filename: harver-vacancies-api-openapi.yml
  format: yaml
  label: Harver vacancies API
  slug: harver-vacancies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-vacancies-api-openapi.yml
- filename: harver-webhook-api-openapi.yml
  format: yaml
  label: Harver webhook API
  slug: harver-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-webhook-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Harver Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Harver secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Harver
provider_slug: harver
scheme_count: 1
schemes:
- content_type: application/x-www-form-urlencoded
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  request_body:
    client_id: '{provided by Harver}'
    client_secret: '{provided by Harver}'
    grant_type: client_credentials
  scopes: []
  token_url: https://api.harver.com/oauth/token
  token_url_test: https://api.harver-test.com/oauth/token
  type: oauth2
  usage: 'Authorization: Bearer {access_token}'
slug: harver-authentication
source_filename: harver-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.harver.com/docs\ndocs: https://api.harver.com/docs#tag/oauth\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_type: Bearer\n  access_token_ttl_seconds: 3600\nnotes: >-\n  The Harver Public API uses OAuth2 client_credentials. The client_id and\n  client_secret are provisioned by Harver per environment (Test / Production);\n  the API is available only to Harver customers. Security schemes are not\n  declared in the components of the published OpenAPI, so this profile is\n  captured from the documented authentication section rather than derived.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.harver.com/oauth/token\n  token_url_test: https://api.harver-test.com/oauth/token\n  grant_type: client_credentials\n  content_type: application/x-www-form-urlencoded\n  request_body:\n    grant_type: client_credentials\n    client_id: '{provided\
  \ by Harver}'\n    client_secret: '{provided by Harver}'\n  usage: 'Authorization: Bearer {access_token}'\n  scopes: []\nenvironments:\n- name: Production\n  base_url: https://api.harver.com\n- name: Test\n  base_url: https://api.harver-test.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/authentication/harver-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- HR
- HR Tech
- Recruiting
- Hiring
- Talent Intelligence
- Pre-Employment Assessment
- Candidate Experience
- Applicant Tracking
---
