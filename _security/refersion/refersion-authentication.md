---
api_key_in: []
api_specs:
- filename: refersion-affiliates-api-openapi.yml
  format: yaml
  label: Refersion Affiliates API
  slug: refersion-affiliates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refersion/refs/heads/main/openapi/refersion-affiliates-api-openapi.yml
- filename: refersion-conversions-api-openapi.yml
  format: yaml
  label: Refersion Conversions API
  slug: refersion-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refersion/refs/heads/main/openapi/refersion-conversions-api-openapi.yml
- filename: refersion-offers-api-openapi.yml
  format: yaml
  label: Refersion Offers API
  slug: refersion-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refersion/refs/heads/main/openapi/refersion-offers-api-openapi.yml
- filename: refersion-reporting-api-openapi.yml
  format: yaml
  label: Refersion Reporting API
  slug: refersion-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refersion/refs/heads/main/openapi/refersion-reporting-api-openapi.yml
auth_types: []
description: Refersion authenticates the REST API and the inbound order-tracking webhook with a static public/secret key PAIR sent as two custom request headers. There is no OAuth 2.0, no OpenID Connect, no bearer token, no mutual TLS and no token exchange of any kind. Note that the published OpenAPI declares NO `securitySchemes` and NO `security` block — the credentials are modelled as ordinary required header PARAMETERS, so automated tooling that reads only securitySchemes will conclude this API is unauthenticated. That is a real defect in the contract, not a gap in this profile.
kind: authentication
layout: security
method: searched
name: Refersion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Refersion declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Refersion
provider_slug: refersion
scheme_count: 2
schemes:
- description: Public half of the key pair, identifying the Refersion account. Example prefix published in the spec is `pub_`. Also used alone, client-side, as `r.pubKey` in the refersion.js tracking snippet.
  example_prefix: pub_
  in: header
  name: Refersion-Public-Key
  required: true
  spec_component: '#/components/parameters/Refersion-Public-Key'
  type: apiKey
- description: Secret half of the key pair. Server-side only — it never appears in any documented client-side snippet.
  example_prefix: sec_
  in: header
  name: Refersion-Secret-Key
  required: true
  spec_component: '#/components/parameters/Refersion-Secret-Key'
  type: apiKey
slug: refersion-authentication
source_filename: refersion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://www.refersion.dev/reference/order-tracking-overview and the provider-published OpenAPI\n  embedded in the ReadMe reference pages (harvested to\n  openapi/_original/refersion-rest-api-readme-harvest.json)\nname: Refersion Authentication\ndescription: >-\n  Refersion authenticates the REST API and the inbound order-tracking webhook with a static\n  public/secret key PAIR sent as two custom request headers. There is no OAuth 2.0, no OpenID\n  Connect, no bearer token, no mutual TLS and no token exchange of any kind. Note that the\n  published OpenAPI declares NO `securitySchemes` and NO `security` block — the credentials are\n  modelled as ordinary required header PARAMETERS, so automated tooling that reads only\n  securitySchemes will conclude this API is unauthenticated. That is a real defect in the\n  contract, not a gap in this profile.\nschemes:\n- name: Refersion-Public-Key\n  type: apiKey\n  in: header\n \
  \ required: true\n  description: >-\n    Public half of the key pair, identifying the Refersion account. Example prefix published in the\n    spec is `pub_`. Also used alone, client-side, as `r.pubKey` in the refersion.js tracking\n    snippet.\n  example_prefix: pub_\n  spec_component: '#/components/parameters/Refersion-Public-Key'\n- name: Refersion-Secret-Key\n  type: apiKey\n  in: header\n  required: true\n  description: >-\n    Secret half of the key pair. Server-side only — it never appears in any documented client-side\n    snippet.\n  example_prefix: sec_\n  spec_component: '#/components/parameters/Refersion-Secret-Key'\napplies_to:\n- surface: REST API v2\n  base_url: https://api.refersion.com/v2\n  headers:\n  - Refersion-Public-Key\n  - Refersion-Secret-Key\n  - Content-Type\n  note: All 15 published operations require both keys plus Content-Type application/json.\n- surface: Inbound order-tracking webhook\n  base_url: https://inbound-webhooks.refersion.com\n  headers:\n  -\
  \ Refersion-Public-Key\n  - Refersion-Secret-Key\n  docs: https://www.refersion.dev/reference/webhook-tracking\n- surface: Client-side tracking (refersion.js)\n  headers: []\n  note: Public key only, assigned to r.pubKey in the browser. The secret key is never exposed here.\n- surface: GraphQL API\n  base_url: https://api.refersion.com/graphql\n  note: >-\n    Documented as available but the endpoint returns HTTP 403 {\"message\":\"Forbidden\"} to an\n    anonymous POST, so the credential form could not be confirmed by probe. The overview page\n    documents no auth mechanism of its own.\n  probed:\n    url: https://api.refersion.com/graphql\n    http_status: 403\n    checked: '2026-08-13'\nkey_management:\n  location: Account > Settings > Refersion API\n  url: https://www.refersion.com/base/settings/integrations/api\n  self_service: true\n  rotation: >-\n    Merchants may use an existing key set or create a new set from the dashboard. No documented\n    programmatic rotation, no expiry,\
  \ no scoping and no per-key permissioning.\n  scopes: none\n  expiry: none\nfailure_modes:\n- status: 401\n  body: '{\"error\": \"Invalid API credentials (error 2).\"}'\n  description: >-\n    Unauthorized — API keys are incorrect. Defined once as\n    #/components/responses/401_Error and $ref'd by every operation.\ngaps:\n- The OpenAPI declares no securitySchemes / security, only header parameters.\n- No OAuth 2.0 or OIDC; therefore no scopes artifact is produced for this provider.\n- Keys are long-lived, unscoped and account-wide — a leaked pair grants the full API surface.\n- The dedicated /reference/authentication docs page exists but is an unedited ReadMe placeholder.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refersion/refs/heads/main/authentication/refersion-authentication.yml
summary_line: 2 schemes
tags:
- Affiliate Marketing
- Influencer Marketing
- E-Commerce
- Referral Tracking
- Commission Management
- Shopify
---
