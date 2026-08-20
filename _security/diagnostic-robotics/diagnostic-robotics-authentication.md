---
api_key_in:
- header
api_specs:
- filename: diagnostic-robotics-precision-population-health-openapi.yml
  format: yaml
  label: Diagnostic Robotics Precision Population Health API
  slug: diagnostic-robotics-precision-population-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-precision-population-health-openapi.yml
- filename: diagnostic-robotics-patient-questionnaire-openapi.yml
  format: yaml
  label: Diagnostic Robotics Patient Questionnaire API
  slug: diagnostic-robotics-patient-questionnaire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-patient-questionnaire-openapi.yml
- filename: diagnostic-robotics-symptom-search-openapi.yml
  format: yaml
  label: Diagnostic Robotics Symptom Search Service
  slug: diagnostic-robotics-symptom-search-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-symptom-search-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Diagnostic Robotics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: Diagnostic Robotics secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: Diagnostic Robotics
provider_slug: diagnostic-robotics
scheme_count: 3
schemes:
- description: Client API key, provided by Diagnostic Robotics, must be supplied with any request
  in: header
  name: apikey
  parameter: x-client
  sources:
  - openapi/diagnostic-robotics-patient-questionnaire-openapi.yml
  - openapi/diagnostic-robotics-symptom-search-openapi.yml
  type: apiKey
- applied_to: 14 of 15 operations in the Precision Population Health spec
  docs_form: 'POST https://[CLIENT].precision-population-health.diagnosticrobotics.com/api/oauth/token with Content-Type application/x-www-form-urlencoded and body client_id={client_id}&client_secret={client_secret}; the response TokenResponse is presented as `Authorization: Bearer {token}` on every subsequent call.'
  flows:
  - flow: password
    scopes: 0
    tokenUrl: /api/oauth/token
  name: OAuth2PasswordBearer
  sources:
  - openapi/diagnostic-robotics-precision-population-health-openapi.yml
  - https://docs.diagnosticrobotics.com/docs/proactive-patient-risk-feed-api/3y8qknbsqo42r-authentication
  type: oauth2
- applied_to: 1 operation (upload_api_v1_dataset__dataset_type__upload_post)
  flows:
  - authorizationUrl: https://digital-outreach.us.auth0.com/authorize?audience=dev-digital-outreach-api-identifier
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://digital-outreach.us.auth0.com/oauth/token
  name: OAuth2AuthorizationCodeBearer
  sources:
  - openapi/diagnostic-robotics-precision-population-health-openapi.yml
  type: oauth2
slug: diagnostic-robotics-authentication
source_filename: diagnostic-robotics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/diagnostic-robotics-patient-questionnaire-openapi.yml, openapi/diagnostic-robotics-precision-population-health-openapi.yml,\n  openapi/diagnostic-robotics-symptom-search-openapi.yml\ndocs: https://docs.diagnosticrobotics.com/docs/proactive-patient-risk-feed-api/3y8qknbsqo42r-authentication\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - password\n  credentials_issued_by: provider\n  self_serve_signup: false\n  note: >-\n    Credentials are never self-serve. The Patient Questionnaire and Symptom Search services take an x-client API\n    key \"provided by Diagnostic Robotics\"; the Precision Population Health service takes an OAuth 2.0 client_id /\n    client_secret pair that Diagnostic Robotics issues per customer, exchanged for a bearer token at\n    POST /api/oauth/token on the customer's own subdomain.\nschemes:\n- name: apikey\n  type: apiKey\n \
  \ in: header\n  parameter: x-client\n  description: Client API key, provided by Diagnostic Robotics, must be supplied with any request\n  sources:\n  - openapi/diagnostic-robotics-patient-questionnaire-openapi.yml\n  - openapi/diagnostic-robotics-symptom-search-openapi.yml\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /api/oauth/token\n    scopes: 0\n  applied_to: 14 of 15 operations in the Precision Population Health spec\n  docs_form: >-\n    POST https://[CLIENT].precision-population-health.diagnosticrobotics.com/api/oauth/token with\n    Content-Type application/x-www-form-urlencoded and body client_id={client_id}&client_secret={client_secret};\n    the response TokenResponse is presented as `Authorization: Bearer {token}` on every subsequent call.\n  sources:\n  - openapi/diagnostic-robotics-precision-population-health-openapi.yml\n  - https://docs.diagnosticrobotics.com/docs/proactive-patient-risk-feed-api/3y8qknbsqo42r-authentication\n\
  - name: OAuth2AuthorizationCodeBearer\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://digital-outreach.us.auth0.com/authorize?audience=dev-digital-outreach-api-identifier\n    tokenUrl: https://digital-outreach.us.auth0.com/oauth/token\n    scopes: 0\n  applied_to: 1 operation (upload_api_v1_dataset__dataset_type__upload_post)\n  sources:\n  - openapi/diagnostic-robotics-precision-population-health-openapi.yml\nx-findings:\n- id: dead-auth0-tenant\n  severity: high\n  detail: >-\n    The published OpenAPI declares an authorizationCode flow against the Auth0 tenant\n    digital-outreach.us.auth0.com. That host no longer resolves as an Auth0 tenant - every discovery path\n    returns HTTP 404 with the body \"Unknown host: digital-outreach.us.auth0.com\". The declared audience\n    (dev-digital-outreach-api-identifier) is also a development identifier. The scheme as published is not\n    usable; the password/client-credentials flow at /api/oauth/token\
  \ is the live path.\n  evidence:\n  - url: https://digital-outreach.us.auth0.com/.well-known/openid-configuration\n    status: 404\n  - url: https://digital-outreach.us.auth0.com/.well-known/oauth-authorization-server\n    status: 404\n  checked: '2026-08-12'\n- id: no-oauth-discovery\n  severity: medium\n  detail: >-\n    No RFC 8414 / OIDC discovery document is served on any Diagnostic Robotics host. The token endpoint is\n    documented only in prose and in the OpenAPI, and tokenUrl is recorded as a relative path (/api/oauth/token)\n    rather than an absolute URL.\n  evidence:\n  - url: https://sandbox.precision-population-health.diagnosticrobotics.com/.well-known/oauth-authorization-server\n    status: 200\n    note: HTTP 200 but the body is the React SPA index.html, not a discovery document\n  checked: '2026-08-12'\nx-evidence:\n- url: https://sandbox.precision-population-health.diagnosticrobotics.com/api/v2/RiskList\n  status: 401\n  body: '{\"detail\":\"Not authenticated\"}'\n\
  - url: https://sandbox.precision-population-health.diagnosticrobotics.com/api/oauth/token\n  status: 405\n  note: GET rejected; endpoint is POST-only, confirming the documented token endpoint is live\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/authentication/diagnostic-robotics-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Health
- Healthcare
- Clinical AI
- Population Health
- Risk Adjustment
- Predictive Analytics
- triage
- FHIR
- Claims Data
- Care Management
- Payers
- Medical Coding
---
