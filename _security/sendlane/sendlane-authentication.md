---
api_key_in:
- header
api_specs:
- filename: sendlane-openapi.yml
  format: yaml
  label: Sendlane API
  slug: sendlane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendlane/refs/heads/main/openapi/sendlane-openapi.yml
auth_types:
- apiKey
description: Auth profile for the Sendlane v2 API. Derived from the two securitySchemes in the published OpenAPI, then upgraded from the provider's own Authentication docs page with the token-issuance procedure and the required Accept header.
kind: authentication
layout: security
method: searched
name: Sendlane Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sendlane secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sendlane
provider_slug: sendlane
scheme_count: 2
schemes:
- default: true
  description: API token sent in the Authorization header with the value "Bearer {apiToken}"
  format: Bearer <YOUR_API_TOKEN>
  in: header
  name: BearerToken
  parameter: Authorization
  sources:
  - openapi/sendlane-openapi.yml
  - https://sendlane.stoplight.io/docs/api-documentation/ZG9jOjk3NDY2OQ-authentication
  type: apiKey
- default: false
  description: API token for another account, sent in the Authorization-Destination header. Names the DESTINATION account of a cross-account operation — used by POST /automations/copy (post-automations-copy) to copy an automation out of the account owning the Authorization token into the account owning this one.
  format: Bearer <OTHER_ACCOUNT_API_TOKEN>
  in: header
  name: OtherAccountBearerToken
  parameter: Authorization-Destination
  sources:
  - openapi/sendlane-openapi.yml
  type: apiKey
slug: sendlane-authentication
source_filename: sendlane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://sendlane.stoplight.io/docs/api-documentation/ZG9jOjk3NDY2OQ-authentication\nderived_from: openapi/sendlane-openapi.yml\ndocs: https://sendlane.stoplight.io/docs/api-documentation/ZG9jOjk3NDY2OQ-authentication\nname: Sendlane API Authentication\ndescription: >-\n  Auth profile for the Sendlane v2 API. Derived from the two securitySchemes in the\n  published OpenAPI, then upgraded from the provider's own Authentication docs page\n  with the token-issuance procedure and the required Accept header.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\n  token_expiry: none documented\n  token_rotation: none documented\nschemes:\n  - name: BearerToken\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: 'Bearer <YOUR_API_TOKEN>'\n    description: API token sent in the Authorization header with the value \"Bearer\
  \ {apiToken}\"\n    default: true\n    sources:\n      - openapi/sendlane-openapi.yml\n      - https://sendlane.stoplight.io/docs/api-documentation/ZG9jOjk3NDY2OQ-authentication\n  - name: OtherAccountBearerToken\n    type: apiKey\n    in: header\n    parameter: Authorization-Destination\n    format: 'Bearer <OTHER_ACCOUNT_API_TOKEN>'\n    description: >-\n      API token for another account, sent in the Authorization-Destination header.\n      Names the DESTINATION account of a cross-account operation — used by\n      POST /automations/copy (post-automations-copy) to copy an automation out of the\n      account owning the Authorization token into the account owning this one.\n    default: false\n    sources:\n      - openapi/sendlane-openapi.yml\nglobal_security:\n  - BearerToken: []\nrequired_headers:\n  - name: Authorization\n    value: 'Bearer <YOUR_API_TOKEN>'\n  - name: Accept\n    value: application/json\n    note: >-\n      The Authentication docs page instructs callers to \"make\
  \ sure to set your content\n      type to json in the header\". Not enforced by the spec, but published as required.\ntoken_issuance:\n  self_service: true\n  steps:\n    - Log in to your Sendlane account.\n    - Navigate to the API section.\n    - Generate a v2 access token.\n    - Click Copy API Token to copy it to your clipboard.\n  source: https://sendlane.stoplight.io/docs/api-documentation/ZG9jOjk3NDY2OQ-authentication\n  note: >-\n    \"Generate a v2 access token\" implies a v1 token type still exists in the\n    dashboard. No v1 retirement date is published.\nobserved:\n  - probe: 'GET https://api.sendlane.com/v2/lists with no Authorization header'\n    date: '2026-08-13'\n    status: 401\n    body: 'Unauthorized.'\n    content_type: text/html; charset=UTF-8\n    www_authenticate: absent\n    note: >-\n      The 401 is text/html, not the documented JSON error envelope, and carries no\n      WWW-Authenticate challenge — so the most common auth failure does not parse as\n      JSON\
  \ and does not advertise the scheme.\nfindings:\n  - >-\n    A single static, account-scoped bearer token with NO scopes. Any credential\n    issued can read every contact and delete lists, contacts, tags, senders and\n    integrations. There is no least-privilege option and no read-only key.\n  - >-\n    No documented expiry, no refresh endpoint, no rotation guidance and no\n    programmatic revocation — key hygiene is entirely manual in the dashboard.\n  - >-\n    No OAuth 2.0 and no OpenID Connect. /.well-known/oauth-authorization-server and\n    /.well-known/openid-configuration return 404 on every Sendlane host (probed\n    2026-08-13), which is consistent with the spec. No scopes artifact is written.\n  - >-\n    The Beacon browser script uses a SEPARATE public \"integration token\"\n    (data-token attribute), which is safe to expose client-side. Do not confuse it\n    with the v2 API bearer token, which is not.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendlane/refs/heads/main/authentication/sendlane-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Email Marketing
- SMS Marketing
- E-Commerce
- Marketing Automation
- Contacts
- Campaigns
- Segmentation
- Consent Management
- Suppression
- Event Tracking
- Revenue Attribution
---
