---
api_key_in:
- header
api_specs:
- filename: moxe-health-claims-api-openapi.yml
  format: yaml
  label: Moxe Health Claims API
  slug: moxe-health-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moxe-health/refs/heads/main/openapi/moxe-health-claims-api-openapi.yml
- filename: moxe-health-patient-api-openapi.yml
  format: yaml
  label: Moxe Health Patient API
  slug: moxe-health-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moxe-health/refs/heads/main/openapi/moxe-health-patient-api-openapi.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Moxe Health Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Moxe Health secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Moxe Health
provider_slug: moxe-health
scheme_count: 2
schemes:
- flows:
  - audience_required: true
    flow: clientCredentials
    scopes: 2
    tokenUrl: https://${environment}-api.moxehealth.com/oauth/token
    token_ttl_seconds: 900
  name: moxe_auth
  sources:
  - openapi/moxe-health-chart-retrieval-initiate-openapi.json
  - openapi/moxe-health-chart-retrieval-status-openapi.json
  - openapi/moxe-health-claim-management-initiate-openapi.json
  - openapi/moxe-health-claim-management-status-openapi.json
  type: oauth2
- in: header
  name: x-api-key
  parameter_name: x-api-key
  sources:
  - openapi/moxe-health-chart-retrieval-initiate-openapi.json
  - openapi/moxe-health-chart-retrieval-status-openapi.json
  - openapi/moxe-health-claim-management-initiate-openapi.json
  - openapi/moxe-health-claim-management-status-openapi.json
  type: apiKey
slug: moxe-health-authentication
source_filename: moxe-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/moxe-health-chart-retrieval-initiate-openapi.json, openapi/moxe-health-chart-retrieval-status-openapi.json,\n  openapi/moxe-health-claim-management-initiate-openapi.json, openapi/moxe-health-claim-management-status-openapi.json\ndocs: https://developer.moxehealth.com/docs/authentication\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  oauth2_flows:\n  - clientCredentials\n  api_key_in:\n  - header\nnotes: >-\n  Every request must present TWO credentials issued by Moxe during partner onboarding:\n  (1) an OAuth2 client-credentials bearer access token, and (2) a static API key. The\n  bearer token is obtained from a Moxe-provided token endpoint by POSTing grant_type=client_credentials\n  with client_id, client_secret, and an audience value (all provided by Moxe). The token\n  response returns access_token, token_type=Bearer, and expires_in=900 (15 minutes). The\n  token is then sent on API calls in a NON-STANDARD header\
  \ named \"Authentication: Bearer\n  {access_token}\" (not the conventional \"Authorization\" header), alongside \"x-api-key:\n  {api_key}\". The OpenAPI additionally declares a custom API Gateway request authorizer\n  (\"${environment}-chart-retrieval-api-authorizer\"). Credentials are not self-serve; they\n  are granted only under a partner onboarding agreement.\nschemes:\n- name: moxe_auth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://${environment}-api.moxehealth.com/oauth/token\n    scopes: 2\n    token_ttl_seconds: 900\n    audience_required: true\n  sources:\n  - openapi/moxe-health-chart-retrieval-initiate-openapi.json\n  - openapi/moxe-health-chart-retrieval-status-openapi.json\n  - openapi/moxe-health-claim-management-initiate-openapi.json\n  - openapi/moxe-health-claim-management-status-openapi.json\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  sources:\n  - openapi/moxe-health-chart-retrieval-initiate-openapi.json\n\
  \  - openapi/moxe-health-chart-retrieval-status-openapi.json\n  - openapi/moxe-health-claim-management-initiate-openapi.json\n  - openapi/moxe-health-claim-management-status-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moxe-health/refs/heads/main/authentication/moxe-health-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Healthcare
- United States
- Interoperability
- Clinical Data
- Payer
- Provider
- EHR
- Health Data Exchange
- Claims
- Risk Adjustment
---
