---
api_key_in:
- header
- query
api_specs:
- filename: miso-public-api-operations-displays-openapi.json
  format: json
  label: MISO Public API - Operations Displays
  slug: miso-public-api-operations-displays
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miso/refs/heads/main/openapi/miso-public-api-operations-displays-openapi.json
- filename: miso-public-api-markets-displays-openapi.json
  format: json
  label: MISO Public API - Markets Displays
  slug: miso-public-api-markets-displays
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miso/refs/heads/main/openapi/miso-public-api-markets-displays-openapi.json
- filename: miso-data-exchange-pricing-api-openapi.json
  format: json
  label: MISO Data Exchange Pricing API
  slug: miso-data-exchange-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miso/refs/heads/main/openapi/miso-data-exchange-pricing-api-openapi.json
- filename: miso-data-exchange-load-generation-interchange-api-openapi.json
  format: json
  label: MISO Data Exchange Load, Generation, and Interchange API
  slug: miso-data-exchange-load-generation-interchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miso/refs/heads/main/openapi/miso-data-exchange-load-generation-interchange-api-openapi.json
auth_types:
- none
- apiKey
- mutualTLS
description: MISO runs three different authentication postures across one profile, and the spread is the point. Most of its surface has no authentication at all — 37 Public API endpoints and the entire bulk market-report archive answer an anonymous GET. The keyed half uses a single Azure API Management subscription key, free and self-serve, with no OAuth, no OpenID Connect, no bearer tokens and no scopes anywhere. The market-participant interface at the far end is mutual-TLS with a client digital certificate. There is no OAuth surface to describe, so no scopes/ artifact exists for this provider — the correct outcome for a key-auth API, not a gap.
kind: authentication
layout: security
method: searched
name: Miso Authentication
name_suffix: Authentication
oauth_flows: []
overview: MISO secures its APIs with none, apiKey, and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MISO
provider_slug: miso
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  preferred: true
  sources:
  - openapi/miso-data-exchange-load-generation-interchange-api-openapi.json
  - openapi/miso-data-exchange-pricing-api-openapi.json
  - https://data-exchange.misoenergy.org/developer/apis?api-version=2022-04-01-preview
  type: apiKey
- in: query
  name: apiKeyQuery
  note: Functional but discouraged — a key in the query string lands in access logs, browser history and referrer headers. Use the header form.
  parameter: subscription-key
  preferred: false
  sources:
  - openapi/miso-data-exchange-load-generation-interchange-api-openapi.json
  - openapi/miso-data-exchange-pricing-api-openapi.json
  type: apiKey
slug: miso-authentication
source_filename: miso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  Derived from openapi/miso-data-exchange-load-generation-interchange-api-openapi.json and\n  openapi/miso-data-exchange-pricing-api-openapi.json, then upgraded from MISO's own\n  documentation: https://help.misoenergy.org/knowledgebase/article/KA-01489/en-us (keys and\n  expiry), https://data-exchange.misoenergy.org/developer/apis?api-version=2022-04-01-preview\n  (subscriptionKeyParameterNames and empty OAuth/OIDC settings), and live anonymous probes of\n  every host on 2026-07-27.\ndocs: https://help.misoenergy.org/knowledgebase/article/KA-01489/en-us\ndescription: >-\n  MISO runs three different authentication postures across one profile, and the spread is the\n  point. Most of its surface has no authentication at all — 37 Public API endpoints and the\n  entire bulk market-report archive answer an anonymous GET. The keyed half uses a single\n  Azure API Management subscription key, free and self-serve, with no OAuth,\
  \ no OpenID Connect,\n  no bearer tokens and no scopes anywhere. The market-participant interface at the far end is\n  mutual-TLS with a client digital certificate. There is no OAuth surface to describe, so no\n  scopes/ artifact exists for this provider — the correct outcome for a key-auth API, not a gap.\nsummary:\n  types: [none, apiKey, mutualTLS]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  scopes: 0\n  openid_connect: false\npostures:\n  - id: anonymous\n    apis:\n      - miso:miso-public-api-operations-displays\n      - miso:miso-public-api-markets-displays\n      - miso:miso-market-reports\n    type: none\n    hosts: [https://public-api.misoenergy.org, https://docs.misoenergy.org]\n    verified: '2026-07-27'\n    evidence: >-\n      Every one of the 37 documented Public API paths returned HTTP 200 with content-type\n      application/json to a plain GET carrying no key, no cookie and no account. Market reports\n      (20260726_da_expost_lmp.csv, 20260726_sr_gfm.xlsx,\
  \ Dead_Node_Reports_Readers_Guide.pdf)\n      downloaded anonymously with HTTP 200.\n  - id: subscription-key\n    apis:\n      - miso:miso-data-exchange-pricing-api\n      - miso:miso-data-exchange-load-generation-interchange-api\n    type: apiKey\n    hosts: [https://apim.misoenergy.org]\n    gateway: Azure API Management\n    self_serve: true\n    approval_required: false\n    verified: '2026-07-27'\n    evidence: >-\n      Anonymous GET to https://apim.misoenergy.org/pricing/v1/day-ahead/2026-07-26/lmp-expost\n      returned HTTP 401 {\"statusCode\": 401, \"message\": \"Access denied due to missing\n      subscription key\"}, while an unknown route on the same gateway returned HTTP 404\n      \"Resource not found\" — the 404/401 split confirms the route exists and is key-gated.\n  - id: client-certificate\n    apis:\n      - miso:miso-mui-2-0-api\n    type: mutualTLS\n    hosts: [https://markets.midwestiso.org, https://cce.midwestiso.org]\n    self_serve: false\n    verified: '2026-07-27'\n\
  \    evidence: >-\n      An anonymous TLS connection to markets.midwestiso.org failed at the handshake with an SSL\n      alert rather than returning any HTTP status — direct evidence of client-certificate\n      enforcement. MISO's MUI 2.0 API User Guide states \"All market participants using the JSON\n      programmatic interface must be registered with MISO.\" The certificate is issued through\n      the MISO Market Portal.\nschemes:\n  - name: apiKeyHeader\n    type: apiKey\n    in: header\n    parameter: Ocp-Apim-Subscription-Key\n    preferred: true\n    sources:\n      - openapi/miso-data-exchange-load-generation-interchange-api-openapi.json\n      - openapi/miso-data-exchange-pricing-api-openapi.json\n      - https://data-exchange.misoenergy.org/developer/apis?api-version=2022-04-01-preview\n  - name: apiKeyQuery\n    type: apiKey\n    in: query\n    parameter: subscription-key\n    preferred: false\n    note: >-\n      Functional but discouraged — a key in the query string lands\
  \ in access logs, browser\n      history and referrer headers. Use the header form.\n    sources:\n      - openapi/miso-data-exchange-load-generation-interchange-api-openapi.json\n      - openapi/miso-data-exchange-pricing-api-openapi.json\nkey_lifecycle:\n  issuance: >-\n    A MISO public-website profile is required first; a MISO Data Exchange account is then\n    created at https://data-exchange.misoenergy.org/ and a subscription taken out on each\n    product. Product metadata returns approvalRequired false, so keys are issued immediately.\n  expiry: >-\n    \"The API keys do not expire or require revalidation, but the accounts they are tied to have\n    account password that expire and require reset after 1 year.\"\n  rotation: Not documented. Azure API Management issues a primary and a secondary key per subscription.\n  scope_of_key: >-\n    Per product. Pricing API and Load/Generation/Interchange API are separate subscriptions with\n    separate keys and separate rate-limit budgets.\n\
  \  revocation: Not documented.\nanomalies:\n  - id: bearer-token-mismatch\n    severity: medium\n    detail: >-\n      All 32 Data Exchange operations declare their 401 as \"Invalid or missing Bearer Token in\n      the Authorization header\". No bearer token, OAuth flow or Authorization header exists\n      anywhere in this API — the portal's own API metadata returns empty\n      oAuth2AuthenticationSettings and empty openidAuthenticationSettings for both APIs. The\n      description is leftover template text and will mislead any client generated from the\n      specification. The real credential is the subscription key.\n  - id: optional-security-requirement\n    severity: low\n    detail: >-\n      Both Data Exchange OpenAPIs declare a root security array of [{}, {apiKeyHeader: []},\n      {apiKeyQuery: []}]. The empty object makes authentication formally optional in the\n      specification, which is not what the gateway enforces — anonymous calls are rejected\n      with 401.\nnot_present:\n\
  \  oauth2: false\n  openid_connect: false\n  jwt: false\n  basic_auth: false\n  hmac_signing: false\n  scopes: false\n  mtls_on_public_apis: false\n  well_known_discovery: >-\n    No /.well-known/openid-configuration and no /.well-known/oauth-authorization-server on any\n    host (all HTTP 404, probed 2026-07-27). See well-known/miso-well-known.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miso/refs/heads/main/authentication/miso-authentication.yml
summary_line: none/apiKey/mutualTLS · 2 schemes
tags:
- Energy
- United States
- Electricity
- Energy Markets
- Grid
- System Operator
- Market Operator
- Wholesale Power
- Open Energy Data
- Renewables
- Solar
- Demand Response
- Utilities
---
