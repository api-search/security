---
api_key_in:
- header
api_specs:
- filename: pverify-authentication-api-openapi.yml
  format: yaml
  label: pVerify Authentication API
  slug: pverify-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-authentication-api-openapi.yml
- filename: pverify-eligibility-api-openapi.yml
  format: yaml
  label: pVerify Eligibility API
  slug: pverify-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-eligibility-api-openapi.yml
- filename: pverify-dental-eligibility-api-openapi.yml
  format: yaml
  label: pVerify Dental Eligibility API
  slug: pverify-dental-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-dental-eligibility-api-openapi.yml
- filename: pverify-insurance-discovery-api-openapi.yml
  format: yaml
  label: pVerify Insurance Discovery API
  slug: pverify-insurance-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-insurance-discovery-api-openapi.yml
- filename: pverify-mbi-lookup-api-openapi.yml
  format: yaml
  label: pVerify MBI Lookup API
  slug: pverify-mbi-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-mbi-lookup-api-openapi.yml
- filename: pverify-patient-demographic-validator-api-openapi.yml
  format: yaml
  label: pVerify Patient Demographic Validator API
  slug: pverify-patient-demographic-validator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-patient-demographic-validator-api-openapi.yml
- filename: pverify-claim-status-api-openapi.yml
  format: yaml
  label: pVerify Claim Status API
  slug: pverify-claim-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-claim-status-api-openapi.yml
- filename: pverify-estimation-api-openapi.yml
  format: yaml
  label: pVerify Patient Cost Estimator API
  slug: pverify-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-estimation-api-openapi.yml
- filename: pverify-payers-api-openapi.yml
  format: yaml
  label: pVerify Payers API
  slug: pverify-payers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-payers-api-openapi.yml
- filename: pverify-cgx-widget-api-openapi.yml
  format: yaml
  label: pVerify CGX Widget API
  slug: pverify-cgx-widget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-cgx-widget-api-openapi.yml
- filename: pverify-same-or-similar-api-openapi.yml
  format: yaml
  label: pVerify Same or Similar API (discontinued)
  slug: pverify-same-or-similar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-same-or-similar-api-openapi.yml
- filename: pverify-cmn-api-openapi.yml
  format: yaml
  label: pVerify CMN API (discontinued)
  slug: pverify-cmn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-cmn-api-openapi.yml
- filename: pverify-snf-api-openapi.yml
  format: yaml
  label: pVerify SNF API (discontinued)
  slug: pverify-snf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-snf-api-openapi.yml
auth_types:
- http
- apiKey
description: 'pVerify uses a two-factor-by-header model: an OAuth2 client-credentials bearer token obtained from POST /Token, sent alongside a Client-API-Id header that identifies the account. Both are required on every call. A small set of "one step" endpoints skips the token entirely and authenticates with Client-API-Id + Client-Secret headers, and one endpoint (GetPayerStatus) is documented as requiring no authentication at all.'
kind: authentication
layout: security
method: searched
name: Pverify Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: pVerify secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: pVerify
provider_slug: pverify
scheme_count: 3
schemes:
- description: 'OAuth2 access token returned by POST /Token, sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_original/pverify-openapi.yml
  type: http
- description: Client API identifier issued by pVerify. Required on every call. pVerify states the header key is case sensitive.
  in: header
  name: clientApiId
  parameter: Client-API-Id
  sources:
  - openapi/_original/pverify-openapi.yml
  type: apiKey
- description: Client secret issued by pVerify. Used by the one-step endpoints (EasyEligibilitySummary) and the premium report endpoints (EligibilityPDFReport, PDFReport/*) in place of a bearer token.
  in: header
  name: clientSecret
  parameter: Client-Secret
  sources:
  - openapi/_original/pverify-openapi.yml
  type: apiKey
slug: pverify-authentication
source_filename: pverify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/_original/pverify-openapi.yml\ndocs: https://postman.pverify.com/\ndescription: >-\n  pVerify uses a two-factor-by-header model: an OAuth2 client-credentials bearer token obtained\n  from POST /Token, sent alongside a Client-API-Id header that identifies the account. Both are\n  required on every call. A small set of \"one step\" endpoints skips the token entirely and\n  authenticates with Client-API-Id + Client-Secret headers, and one endpoint (GetPayerStatus) is\n  documented as requiring no authentication at all.\nsummary:\n  types: [http, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  oauth2_scopes: 0\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth2 access token returned by POST /Token, sent as `Authorization: Bearer <token>`.'\n  sources: [openapi/_original/pverify-openapi.yml]\n- name: clientApiId\n  type: apiKey\n  in: header\n  parameter: Client-API-Id\n\
  \  description: >-\n    Client API identifier issued by pVerify. Required on every call. pVerify states the header key\n    is case sensitive.\n  sources: [openapi/_original/pverify-openapi.yml]\n- name: clientSecret\n  type: apiKey\n  in: header\n  parameter: Client-Secret\n  description: >-\n    Client secret issued by pVerify. Used by the one-step endpoints (EasyEligibilitySummary) and\n    the premium report endpoints (EligibilityPDFReport, PDFReport/*) in place of a bearer token.\n  sources: [openapi/_original/pverify-openapi.yml]\ntoken_endpoint:\n  url: https://api.pverify.com/Token\n  test_url: https://testapi.pverify.com/Token\n  method: POST\n  content_type: application/x-www-form-urlencoded\n  grant_type: client_credentials\n  parameters: [Client_Id, Client_Secret, grant_type]\n  response_fields: [access_token, token_type, expires_in]\n  note: >-\n    A client-credentials grant, but with non-standard parameter names — pVerify sends Client_Id /\n    Client_Secret rather than\
  \ RFC 6749's client_id / client_secret, and there is no scope parameter.\n    Token lifetime is returned in expires_in; no fixed value is published.\nscopes:\n  published: false\n  note: >-\n    No OAuth scopes exist. Product entitlements (eligibility, claim status, insurance discovery,\n    MBI, pDV) are attached to the account contract, not to the token, so scopes/ is deliberately\n    not emitted for this provider.\nunauthenticated_operations:\n- {operationId: getPayerStatus, path: /api/GetPayerStatus, note: 'pVerify documents \"this API call does not require authentication\"'}\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/authentication/pverify-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Healthcare
- Insurance
- Eligibility
- Claims
- EDI
- 270/271
- 276/277
- Revenue Cycle
- Medicare
- Payers
- Insurance Discovery
- Patient Estimation
- HIPAA
- Dental
---
