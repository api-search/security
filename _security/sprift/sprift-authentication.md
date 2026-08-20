---
api_key_in:
- header
api_specs:
- filename: sprift-openapi.json
  format: json
  label: Sprift Property API
  slug: sprift-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-openapi.json
- filename: sprift-openapi.json
  format: json
  label: Sprift Property V2 API
  slug: sprift-property-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-openapi.json
- filename: sprift-openapi.json
  format: json
  label: Sprift Search API
  slug: sprift-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-openapi.json
- filename: sprift-openapi.json
  format: json
  label: Sprift Insider API
  slug: sprift-insider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-openapi.json
- filename: sprift-openapi.json
  format: json
  label: Sprift Report Share API
  slug: sprift-share-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-openapi.json
- filename: sprift-openapi.json
  format: json
  label: Sprift User API
  slug: sprift-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sprift Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sprift secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sprift
provider_slug: sprift
scheme_count: 2
schemes:
- applies_to: all 27 operations in the published contract
  in: header
  name: SPRIFT-API-KEY
  note: This is the real, operative scheme. Every one of the 27 operations in the harvested Swagger 2.0 document declares a REQUIRED header parameter named SPRIFT-API-KEY. It is declared as an ordinary header parameter, not as a securityDefinition, so generic tooling that reads only securityDefinitions will miss it.
  parameter_name: SPRIFT-API-KEY
  required: true
  sources:
  - openapi/sprift-openapi.json
  type: apiKey
- name: auth
  note: 'Declared in securityDefinitions and applied globally via security [{"auth": []}], but contradicted by every operation''s SPRIFT-API-KEY header parameter and by the Bearer token described on the product page. Recorded verbatim from the harvested contract; not corrected.'
  scheme: basic
  sources:
  - openapi/sprift-openapi.json
  type: http
slug: sprift-authentication
source_filename: sprift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/sprift-openapi.json\ndocs: https://sprift.com/en/livechatacademy/api-key\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  effective_scheme: custom API key header (SPRIFT-API-KEY)\n  self_serve: false\nschemes:\n- name: SPRIFT-API-KEY\n  type: apiKey\n  in: header\n  parameter_name: SPRIFT-API-KEY\n  required: true\n  applies_to: all 27 operations in the published contract\n  sources:\n  - openapi/sprift-openapi.json\n  note: >-\n    This is the real, operative scheme. Every one of the 27 operations in the\n    harvested Swagger 2.0 document declares a REQUIRED header parameter named\n    SPRIFT-API-KEY. It is declared as an ordinary header parameter, not as a\n    securityDefinition, so generic tooling that reads only securityDefinitions will\n    miss it.\n- name: auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/sprift-openapi.json\n  note: >-\n    Declared in\
  \ securityDefinitions and applied globally via security [{\"auth\": []}],\n    but contradicted by every operation's SPRIFT-API-KEY header parameter and by the\n    Bearer token described on the product page. Recorded verbatim from the harvested\n    contract; not corrected.\ncontract_defect: >-\n  Sprift publishes three mutually inconsistent statements of its own auth model:\n  (1) HTTP Basic, in the Swagger securityDefinitions; (2) a custom SPRIFT-API-KEY\n  header, in every operation's parameters; (3) a Bearer token with an\n  sk_live_sprift_ prefix, on the Data and API product page. The header parameter is\n  the one that matches observed behaviour of the documented v1 host.\nmarketing_claim:\n  source: https://sprift.com/data-and-api\n  quote: >-\n    Sprift uses token-based authentication. Existing subscribers can generate an API\n    key instantly from their account settings. No new contracts, no procurement\n    delays. Navigate to Settings, then Developer, then API Keys. Click\
  \ \"Generate new\n    key\". Include your key as a Bearer token in every request. All endpoints are\n    HTTPS only.\n  key_format_shown: sk_live_sprift_ prefix, remainder masked on the page\n  verified: false\n  note: >-\n    Could not be verified — the Settings > Developer > API Keys screen sits behind\n    https://sprift.com/dashboard/login. This describes the advertised, uncontracted\n    /api/v2 family, not the published v1 contract.\ncredential_issuance:\n  self_serve_signup: false\n  process: >-\n    Become a Sprift subscriber first (book a demo — pricing is quoted per branch and\n    is not published), then email customer.success@sprift.com with your full name and\n    company, a description of the intended use case, and the systems you plan to\n    integrate with. Sprift reviews the request, and API access \"may require an\n    additional agreement depending on your subscription.\"\n  contact: customer.success@sprift.com\n  docs: https://sprift.com/en/livechatacademy/api-key\n\
  \  register_endpoints_checked:\n  - url: https://sprift.com/dashboard/register\n    status: 404\n  - url: https://sprift.com/dashboard/signup\n    status: 404\nend_user_login:\n  operations:\n  - Login\n  - Logout\n  path: POST /user/login, GET /user/logout\n  purpose: >-\n    Not the API authentication path. The contract states: \"You do not need to call\n    this Endpoint with your API username and password in order to use the API. This\n    Endpoint is intended to those who want to add Sprift platform into their\n    platforms using an iFrame and let Sprift users to login to Sprift.\" A partner\n    platform authenticates a Sprift end user on the partner's behalf; the call itself\n    still requires the SPRIFT-API-KEY header.\n  returns: status, token, expires, url, telephone, email (inline_response_200_1)\nopenid_connect:\n  present: false\n  evidence: https://sprift.com/.well-known/openid-configuration returns HTTP 404\noauth2:\n  present: false\n  evidence: >-\n    no oauth2 securityScheme\
  \ in the contract; no OAuth documentation on any Sprift\n    surface; scopes/ artifact intentionally absent\nmtls:\n  present: false\nanonymous_behaviour:\n- url: https://sprift.com/dashboard/api/v1/\n  status: 401\n  body: '{\"status\":false,\"error\":\"Unauthorized\"}'\n- url: https://sprift.com/dashboard/api/v1/search?phrase=SW1A\n  header: 'SPRIFT-API-KEY: invalid-test-key'\n  status: 401\n  body: '{\"status\":false,\"error\":\"Unauthorized\"}'\n- url: https://api.sprift.com/\n  status: 403\n  body: '{\"message\":\"Missing Authentication Token\"}'\n  note: AWS API Gateway default (x-amzn-errortype MissingAuthenticationTokenException)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/authentication/sprift-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Data
- Property Listings
- Valuation
- AVM
- Land Registry
- Conveyancing
- Rentals
- Mortgage
---
