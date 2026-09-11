---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: first-american-financial-title-settlement-openapi.yml
  format: yaml
  label: First American Title & Settlement (Mortgage Services) API
  slug: first-american-financial-title-settlement
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-title-settlement-openapi.yml
- filename: first-american-financial-property-openapi.yml
  format: yaml
  label: First American Property API
  slug: first-american-financial-property
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-property-openapi.yml
- filename: first-american-financial-ownership-openapi.yml
  format: yaml
  label: First American Ownership API
  slug: first-american-financial-ownership
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-ownership-openapi.yml
- filename: first-american-financial-occupancy-openapi.yml
  format: yaml
  label: First American Occupancy API
  slug: first-american-financial-occupancy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-occupancy-openapi.yml
- filename: first-american-financial-identity-openapi.yml
  format: yaml
  label: First American Identity API
  slug: first-american-financial-identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-identity-openapi.yml
- filename: first-american-financial-bankruptcy-openapi.yml
  format: yaml
  label: First American Bankruptcy API
  slug: first-american-financial-bankruptcy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-bankruptcy-openapi.yml
- filename: first-american-financial-4506c-openapi.yml
  format: yaml
  label: First American 4506-C Tax Transcript API
  slug: first-american-financial-4506c
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-4506c-openapi.yml
- filename: first-american-financial-reverse-phone-openapi.yml
  format: yaml
  label: First American Reverse Phone Search API
  slug: first-american-financial-reverse-phone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-reverse-phone-openapi.yml
- filename: first-american-financial-reverse-address-openapi.yml
  format: yaml
  label: First American Reverse Address Search API
  slug: first-american-financial-reverse-address
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-reverse-address-openapi.yml
- filename: first-american-financial-scra-openapi.yml
  format: yaml
  label: First American Active Duty SCRA Search API
  slug: first-american-financial-scra
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-scra-openapi.yml
- filename: first-american-financial-income-estimate-openapi.yml
  format: yaml
  label: First American Income Estimate API
  slug: first-american-financial-income-estimate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-income-estimate-openapi.yml
- filename: first-american-financial-liens-judgments-fcra-openapi.yml
  format: yaml
  label: First American Liens & Judgments (FCRA) API
  slug: first-american-financial-liens-judgments-fcra
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-liens-judgments-fcra-openapi.yml
- filename: first-american-financial-liens-judgments-non-fcra-openapi.yml
  format: yaml
  label: First American Liens & Judgments (Non-FCRA) API
  slug: first-american-financial-liens-judgments-non-fcra
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-liens-judgments-non-fcra-openapi.yml
- filename: first-american-financial-watchlist-openapi.yml
  format: yaml
  label: First American Watchlist API
  slug: first-american-financial-watchlist
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-watchlist-openapi.yml
- filename: first-american-financial-nmls-openapi.yml
  format: yaml
  label: First American NMLS License Verification API
  slug: first-american-financial-nmls
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-nmls-openapi.yml
- filename: first-american-financial-clearsearch-openapi.yml
  format: yaml
  label: First American ClearSearch API
  slug: first-american-financial-clearsearch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-clearsearch-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: First American Financial Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: First American Financial secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: First American Financial
provider_slug: first-american-financial
scheme_count: 4
schemes:
- aliases:
  - X-App-Id
  declared_as: required header parameter (not a securityDefinition)
  description: Application ID. Issued per App in the Digital Gateway portal after an access request is approved. Sent on EVERY Digital Gateway data-service call.
  in: header
  name: x-app-id
  operations: 70
  parameter: x-app-id
  sources:
  - openapi/first-american-financial-4506c-openapi.yml
  - openapi/first-american-financial-bankruptcy-openapi.yml
  - openapi/first-american-financial-clearsearch-openapi.yml
  - openapi/first-american-financial-identity-openapi.yml
  - openapi/first-american-financial-income-estimate-openapi.yml
  - openapi/first-american-financial-liens-judgments-fcra-openapi.yml
  - openapi/first-american-financial-liens-judgments-non-fcra-openapi.yml
  - openapi/first-american-financial-nmls-openapi.yml
  - openapi/first-american-financial-occupancy-openapi.yml
  - openapi/first-american-financial-ownership-openapi.yml
  - openapi/first-american-financial-property-openapi.yml
  - openapi/first-american-financial-reverse-address-openapi.yml
  - openapi/first-american-financial-reverse-phone-openapi.yml
  - openapi/first-american-financial-scra-openapi.yml
  - openapi/first-american-financial-watchlist-openapi.yml
  type: apiKey
- aliases:
  - X-App-Key
  declared_as: required header parameter (not a securityDefinition)
  description: Application Key, the secret half of the App credential pair. Paired with x-app-id on every data-service call. An invalid pair returns HTTP 401 "Invalid App ID or App Key".
  in: header
  name: x-app-key
  operations: 70
  parameter: x-app-key
  sources:
  - see x-app-id
  type: apiKey
- bearerFormat: JWT
  description: OAuth (a.k.a JWT) Authentication is mandatory. Applied to all 16 non-token operations of the Title & Settlement (Mortgage Services) API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/first-american-financial-title-settlement-openapi.yml
  type: http
- flow: clientCredentials
  name: oauth2-client-credentials
  request_fields:
  - client_id
  - client_secret
  - scope
  - grant_type
  scopes_note: '`scope` is a REQUIRED form field on the token request but no scope values are published anywhere. No scopes/ artifact is written rather than invent one.'
  scopes_published: false
  sources:
  - openapi/first-american-financial-title-settlement-openapi.yml
  token_endpoint: POST /api/token
  token_endpoint_note: The demonstration host in the spec is https://lvis-oauth-swagger.lvisqa.firstam.com and is explicitly marked "THIS ENDPOINT IS FOR DEMONSTRATION PURPOSES ONLY". The real authentication URL is issued privately - the spec says to contact LVIS.support@firstam.com to obtain the URL along with client_id, client_secret, scope and grant_type.
  type: oauth2
slug: first-american-financial-authentication
source_filename: first-american-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: openapi/ — 16 harvested Digital Gateway specifications\ndocs: https://developer.firstam.io/api/docs\nnote: >-\n  Upgraded from the mechanical derive. The derive found only the one declared securityScheme\n  (Title & Settlement's bearer JWT) because the fifteen Swagger 2.0 data-service specs carry no\n  `securityDefinitions` block at all — they express credentials as REQUIRED HEADER PARAMETERS on\n  every operation instead. That is a real, documented API-key scheme (140 header-parameter\n  declarations across 70 operations) and it would have scored as \"no authentication\" had it been\n  left to the spec's own security block.\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\nschemes:\n  - name: x-app-id\n    type: apiKey\n    in: header\n    parameter: x-app-id\n    aliases: [X-App-Id]\n    description: >-\n      Application ID. Issued per App in the Digital Gateway portal\
  \ after an access request is\n      approved. Sent on EVERY Digital Gateway data-service call.\n    declared_as: required header parameter (not a securityDefinition)\n    operations: 70\n    sources:\n      - openapi/first-american-financial-4506c-openapi.yml\n      - openapi/first-american-financial-bankruptcy-openapi.yml\n      - openapi/first-american-financial-clearsearch-openapi.yml\n      - openapi/first-american-financial-identity-openapi.yml\n      - openapi/first-american-financial-income-estimate-openapi.yml\n      - openapi/first-american-financial-liens-judgments-fcra-openapi.yml\n      - openapi/first-american-financial-liens-judgments-non-fcra-openapi.yml\n      - openapi/first-american-financial-nmls-openapi.yml\n      - openapi/first-american-financial-occupancy-openapi.yml\n      - openapi/first-american-financial-ownership-openapi.yml\n      - openapi/first-american-financial-property-openapi.yml\n      - openapi/first-american-financial-reverse-address-openapi.yml\n\
  \      - openapi/first-american-financial-reverse-phone-openapi.yml\n      - openapi/first-american-financial-scra-openapi.yml\n      - openapi/first-american-financial-watchlist-openapi.yml\n  - name: x-app-key\n    type: apiKey\n    in: header\n    parameter: x-app-key\n    aliases: [X-App-Key]\n    description: >-\n      Application Key, the secret half of the App credential pair. Paired with x-app-id on every\n      data-service call. An invalid pair returns HTTP 401 \"Invalid App ID or App Key\".\n    declared_as: required header parameter (not a securityDefinition)\n    operations: 70\n    sources: [see x-app-id]\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      OAuth (a.k.a JWT) Authentication is mandatory. Applied to all 16 non-token operations of the\n      Title & Settlement (Mortgage Services) API.\n    sources:\n      - openapi/first-american-financial-title-settlement-openapi.yml\n  - name: oauth2-client-credentials\n\
  \    type: oauth2\n    flow: clientCredentials\n    token_endpoint: POST /api/token\n    token_endpoint_note: >-\n      The demonstration host in the spec is https://lvis-oauth-swagger.lvisqa.firstam.com and is\n      explicitly marked \"THIS ENDPOINT IS FOR DEMONSTRATION PURPOSES ONLY\". The real authentication\n      URL is issued privately - the spec says to contact LVIS.support@firstam.com to obtain the URL\n      along with client_id, client_secret, scope and grant_type.\n    request_fields: [client_id, client_secret, scope, grant_type]\n    scopes_published: false\n    scopes_note: >-\n      `scope` is a REQUIRED form field on the token request but no scope values are published\n      anywhere. No scopes/ artifact is written rather than invent one.\n    sources:\n      - openapi/first-american-financial-title-settlement-openapi.yml\nonboarding:\n  self_service: false\n  steps:\n    - Sign up at https://developer.firstam.io/signup (two-factor by email).\n    - Account reviewed by\
  \ a Digital Gateway administrator; access granted within 1-2 business days.\n    - Create an App, then request access to specific APIs; approval may be automatic or administrator-gated.\n    - App ID and App Key appear in the App's Credentials section once approved.\n    - Production access additionally requires the First American relationship team and may require a contract and/or SOW.\n  contact: DigitalGateway@firstam.io\nadditional:\n  shared_secret:\n    documented: true\n    description: >-\n      The glossary documents a Shared Secret Key used for message-level symmetric cryptography on\n      some APIs, assigned in the portal. Not expressed in any harvested contract.\n    source: https://developer.firstam.io/api/docs\n  app_source_header:\n    documented: true\n    description: >-\n      'AppSource' is required for customers using source-level credentials on the Title & Settlement\n      document, message and cancel operations.\n    source: openapi/first-american-financial-title-settlement-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/authentication/first-american-financial-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Title Insurance
- Real-Estate
- Settlement Services
- Financial-Services
- Mortgage
- Property Data
- Identity Verification
- Regulatory Compliance
- Fortune 1000
---
