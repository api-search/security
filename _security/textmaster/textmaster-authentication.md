---
api_key_in: []
api_specs:
- filename: textmaster-api-v1-openapi.yml
  format: yaml
  label: TextMaster API v1
  slug: textmaster-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-api-v1-openapi.yml
auth_types:
- oauth2
- custom-signature
description: ''
kind: authentication
layout: security
method: searched
name: Textmaster Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: TextMaster secures its APIs with oauth2 and custom-signature across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: TextMaster
provider_slug: textmaster
scheme_count: 2
schemes:
- app_model: OAuth Apps are registered from the TextMaster application under "API & Loop" -> "View OAuth Applications". Each app has a client_id, client_secret and a registered callback URL. An OAuth App acts as the authenticated user across all of TextMaster and, once granted, receives permissions to every project that user can access.
  authorization_host_discrepancy: The spec names https://api.textmaster.com/oauth/authorize; the scopes documentation and the published Postman collection both use the application host (https://app.textmaster.com/oauth/authorize, and {{baseUrl}}/oauth/authorize where baseUrl is the API host). Both hosts are TextMaster's. Recorded rather than resolved — a client should follow the docs.
  description: OAuth2 Bearer token authentication
  flows:
  - authorizationUrl: https://api.textmaster.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://api.textmaster.com/oauth/token
    scopes: 3
    scopes_note: The spec's flow `scopes` map declares only the three preferred_author scopes, but operation `security[]` requirements reference 21 distinct scopes and the docs publish a 20-row scope table including `public`. The full union of 22 scopes is in scopes/textmaster-scopes.yml.
    tokenUrl: https://api.textmaster.com/oauth/token
  name: oauth2
  refresh_tokens: true
  revocable_by_user: true
  sources:
  - openapi/textmaster-api-v1-openapi.yml
  - https://developer.textmaster.com/apps/about-oauth-apps
  - https://developer.textmaster.com/apps/building-oauth-apps/scopes-for-oauth-apps
  token_delivery:
    format: Bearer <ACCESS-TOKEN>
    header: Authorization
    provider_recommendation: '"TextMaster recommends sending OAuth tokens using the Authorization header."'
  type: oauth2
  user_editable_scopes: true
  user_editable_scopes_note: Users may grant fewer scopes than requested and may edit token scopes after the flow completes, so the granted `scope` attribute on the token must be read rather than assumed.
- description: Legacy per-user key-pair strategy. The client computes SHA-1 over the concatenation of the API secret and a UTC timestamp, then sends three headers. The signature is valid for five minutes after creation. Keys are read from the TextMaster application's "API & Loop" page.
  headers:
  - meaning: The account's public API key.
    name: Apikey
  - meaning: 'UTC timestamp, format: YYYY-MM-DD HH:MM:SS'
    name: Date
  - meaning: SHA-1 hex digest of (api_secret + date)
    name: Signature
  in: header
  name: signature
  provider_guidance: '"TextMaster discourages using the signature strategy to authenticate production applications to the API. Clients should use OAuth2 Apps instead." The quick-start repeats the warning: signature is for test purposes only.'
  signature_algorithm: sha1(api_secret || date)
  sources:
  - https://developer.textmaster.com/overview/authentication
  - https://developer.textmaster.com/quick-start
  spec_declared: false
  type: apiKey
  validity_seconds: 300
  verification_endpoint: https://api.textmaster.com/test
slug: textmaster-authentication
source_filename: textmaster-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: openapi/textmaster-api-v1-openapi.yml\ndocs: https://developer.textmaster.com/overview/authentication\nchecked: '2026-08-17'\nsummary:\n  types:\n  - oauth2\n  - custom-signature\n  oauth2_flows:\n  - authorizationCode\n  note: >-\n    The OpenAPI declares ONE security scheme (oauth2, authorizationCode). The developer portal\n    documents a SECOND, spec-undeclared strategy — a custom HMAC-style \"Signature\" scheme using\n    Apikey / Date / Signature request headers — which the provider itself marks as test-only and\n    discourages for production. Both are recorded here; the signature scheme is the reason this\n    file is `searched` rather than the mechanically `derived` baseline.\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.textmaster.com/oauth/authorize\n    tokenUrl: https://api.textmaster.com/oauth/token\n    refreshUrl: https://api.textmaster.com/oauth/token\n\
  \    scopes: 3\n    scopes_note: >-\n      The spec's flow `scopes` map declares only the three preferred_author scopes, but operation\n      `security[]` requirements reference 21 distinct scopes and the docs publish a 20-row scope\n      table including `public`. The full union of 22 scopes is in scopes/textmaster-scopes.yml.\n  description: OAuth2 Bearer token authentication\n  token_delivery:\n    header: Authorization\n    format: 'Bearer <ACCESS-TOKEN>'\n    provider_recommendation: >-\n      \"TextMaster recommends sending OAuth tokens using the Authorization header.\"\n  app_model: >-\n    OAuth Apps are registered from the TextMaster application under \"API & Loop\" ->\n    \"View OAuth Applications\". Each app has a client_id, client_secret and a registered callback\n    URL. An OAuth App acts as the authenticated user across all of TextMaster and, once granted,\n    receives permissions to every project that user can access.\n  refresh_tokens: true\n  revocable_by_user: true\n\
  \  user_editable_scopes: true\n  user_editable_scopes_note: >-\n    Users may grant fewer scopes than requested and may edit token scopes after the flow\n    completes, so the granted `scope` attribute on the token must be read rather than assumed.\n  authorization_host_discrepancy: >-\n    The spec names https://api.textmaster.com/oauth/authorize; the scopes documentation and the\n    published Postman collection both use the application host\n    (https://app.textmaster.com/oauth/authorize, and {{baseUrl}}/oauth/authorize where baseUrl is\n    the API host). Both hosts are TextMaster's. Recorded rather than resolved — a client should\n    follow the docs.\n  sources:\n  - openapi/textmaster-api-v1-openapi.yml\n  - https://developer.textmaster.com/apps/about-oauth-apps\n  - https://developer.textmaster.com/apps/building-oauth-apps/scopes-for-oauth-apps\n- name: signature\n  type: apiKey\n  in: header\n  spec_declared: false\n  description: >-\n    Legacy per-user key-pair strategy. The\
  \ client computes SHA-1 over the concatenation of the\n    API secret and a UTC timestamp, then sends three headers. The signature is valid for five\n    minutes after creation. Keys are read from the TextMaster application's \"API & Loop\" page.\n  headers:\n  - name: Apikey\n    meaning: The account's public API key.\n  - name: Date\n    meaning: 'UTC timestamp, format: YYYY-MM-DD HH:MM:SS'\n  - name: Signature\n    meaning: SHA-1 hex digest of (api_secret + date)\n  signature_algorithm: sha1(api_secret || date)\n  validity_seconds: 300\n  provider_guidance: >-\n    \"TextMaster discourages using the signature strategy to authenticate production applications\n    to the API. Clients should use OAuth2 Apps instead.\" The quick-start repeats the warning:\n    signature is for test purposes only.\n  verification_endpoint: https://api.textmaster.com/test\n  sources:\n  - https://developer.textmaster.com/overview/authentication\n  - https://developer.textmaster.com/quick-start\nunauthenticated_surface:\n\
  \  note: >-\n    Two surfaces need no credentials at all. Recorded because an agent can reach them with no\n    onboarding.\n  endpoints:\n  - path: /ping\n    method: GET\n    probed_status: 200\n    probed: '2026-08-17'\n    response: '{\"message\":\"Textmaster API at your service\"}'\n  - path: /v1/public/*\n    method: GET\n    note: >-\n      categories, countries, expertises (+ sub_expertises), languages and locales carry no\n      `security[]` requirement in the spec. The docs assign these to the default `public` scope.\noauth_error_envelope:\n  shape: '{\"error\": \"...\", \"error_description\": \"...\"}'\n  documented_codes:\n  - code: invalid_client\n    meaning: client_id and/or client_secret are incorrect.\n  - code: invalid_grant\n    meaning: >-\n      Authorization code / refresh token invalid, expired, revoked, or redirect_uri mismatch.\n  - code: invalid_token\n    meaning: The access token is invalid (returned as 401/403 on API calls).\n  see: errors/textmaster-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/authentication/textmaster-authentication.yml
summary_line: oauth2/custom-signature · 2 schemes
tags:
- Company
- Translation
- Localization
- Language Services
- Copywriting
- Proofreading
- Machine Translation
- Content Production
- Translation Memory
- Glossary
- Ecommerce Localization
- Product Information Management
- Webhook
- Authentication
- Software-as-a-Service
---
