---
anonymous_access: false
api_key_in: []
api_specs:
- filename: franklin-resources-detailed-product-apis-openapi.yml
  format: yaml
  label: Franklin Templeton Detailed Product APIs
  slug: franklin-resources-detailed-product-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/franklin-resources/refs/heads/main/openapi/franklin-resources-detailed-product-apis-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: derived
name: Franklin Resources Authentication
name_suffix: Authentication
oauth_flows: []
overview: Franklin Resources declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Franklin Resources
provider_slug: franklin-resources
scheme_count: 0
schemes: []
slug: franklin-resources-authentication
source_filename: franklin-resources-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: derived\nsource: >-\n  openapi/_original/franklin-resources-productionproductapi-1.0.0.json (Franklin Templeton's own\n  Swagger 2.0 \"Detailed Product APIs\"), cross-read against the archived developer-portal routes\n  /user/register and /user/login at developer.franklintempleton.com.\nrevised: '2026-09-10'\nsummary: >-\n  The contract declares NO `securityDefinitions` block at all. Authentication is expressed only as\n  a REQUIRED `Authorization` header parameter on every one of the 7 operations, defaulted in the\n  spec to the literal string \"Bearer <Access_Token>\" with the description \"Access Token (Note:Need\n  to pass Access token, by generating through postman)\". That is a bearer-token scheme documented\n  by convention rather than declared, which is why the automated securityScheme derivation finds\n  nothing here: a machine reading this contract cannot tell how to obtain a token, only that one is\n  needed.\ndeclared_security_schemes:\
  \ []\nobserved_schemes:\n  - id: authorization-bearer-header\n    type: http\n    scheme: bearer\n    in: header\n    name: Authorization\n    declared_in_spec: false\n    expressed_as: required header parameter on every operation\n    spec_default: 'Bearer <Access_Token>'\n    spec_description: 'Access Token (Note:Need to pass Access token, by generating through postman)'\n    applies_to:\n      - GetFundsDetails\n      - GetInvestmentTeam\n      - GetFundNAV\n      - GetDistributionRate\n      - GetNAVHistory\n      - GetDistributionHistory\n      - GetProductAUM\n    token_endpoint: not documented\n    note: >-\n      No token, authorize, refresh or introspection endpoint appears anywhere in the contract. The\n      only issuance instruction Franklin Templeton published is \"generate it through Postman\",\n      which presupposes a credential handed out through the (now-retired) portal registration flow.\n  - id: x-ft-api-key\n    type: apiKey\n    in: header\n    name: X-FT-API-KEY\n\
  \    declared_in_spec: false\n    applies_to: []\n    seen_in: >-\n      A sibling Franklin Templeton API-program Swagger document (the account-opening surface) makes\n      `X-FT-API-KEY` a required header alongside the bearer token. It does NOT appear on the fund\n      data operations captured in this repo, so it is recorded as an observed program-wide\n      convention, not as a scheme on this API.\n    confidence: medium\nonboarding:\n  self_service: false\n  registration_url: http://developer.franklintempleton.com/user/register\n  registration_status: >-\n    RETIRED. The registration and login routes are archived (2019-07-21 through 2023-03-13) and the\n    host has no DNS A record as of 2026-09-10. There is no way to obtain a credential today.\n  contact: WebAPISupport@franklintempleton.com\noauth2:\n  present: false\n  note: No oauth2 flow, no scope map, no authorization or token URL. No scopes/ artifact is written.\nmtls:\n  present: false\nopenid_connect:\n  present: false\n\
  gaps:\n  - Auth is not machine-declared — an agent reading this contract cannot discover the scheme.\n  - No token endpoint, no credential-lifetime statement, no refresh mechanism.\n  - No scopes, so no least-privilege story for a read-only fund data API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/franklin-resources/refs/heads/main/authentication/franklin-resources-authentication.yml
summary_line: 0 schemes
tags:
- Fortune 500
- Investment Management
- Asset Management
- Financial-Services
- Mutual Funds
- Exchange Traded Funds
- Fund Data
- Market Data
---
