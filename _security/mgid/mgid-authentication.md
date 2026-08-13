---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mgid Authentication
name_suffix: Authentication
oauth_flows: []
overview: MGID secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MGID
provider_slug: mgid
scheme_count: 1
schemes:
- applies_to:
  - mgid:mgid-advertiser-api
  - mgid:mgid-publisher-api
  - mgid:mgid-agency-api
  description: A single opaque 32-character token identifies the account. The docs state "the Mgid REST API uses a unique token consisting of 32 characters which is passed in client's request Authorization header" and "You should get a valid token from the dashboard."
  expiry_documented: false
  format: Bearer {token}
  in: header
  issuance: manual
  issuance_channel: MGID dashboard (self-serve UI)
  name: BearerToken
  parameter_name: Authorization
  rotation_documented: false
  scopes: []
  sources:
  - https://help.mgid.com/api-advertisers/
  - https://help.mgid.com/api-publishers
  - https://help.mgid.com/api-ra
  token_endpoint: null
  token_endpoint_note: No machine-readable token/credential-exchange endpoint is documented on any of the three reference pages. Tokens are copied out of the dashboard by a human; there is no documented programmatic rotation, refresh or revocation call.
  token_length: 32
  type: apiKey
slug: mgid-authentication
source_filename: mgid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://help.mgid.com/api-advertisers/\ndocs:\n  - https://help.mgid.com/api-advertisers/\n  - https://help.mgid.com/api-publishers\n  - https://help.mgid.com/api-ra\nnote: >-\n  MGID publishes no OpenAPI, so this profile could not be derived mechanically\n  from securitySchemes. It is transcribed from the three published REST API\n  reference pages on help.mgid.com, which all document the same single auth\n  model. Probing https://api.mgid.com/v1/ anonymously returns HTTP 401 with the\n  body {\"errors\":\"Authentication token is missing\"}, which confirms the scheme is\n  enforced at the live API host.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  scopes_supported: false\nschemes:\n  - name: BearerToken\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    format: 'Bearer {token}'\n    token_length: 32\n    description:\
  \ >-\n      A single opaque 32-character token identifies the account. The docs state\n      \"the Mgid REST API uses a unique token consisting of 32 characters which is\n      passed in client's request Authorization header\" and \"You should get a\n      valid token from the dashboard.\"\n    issuance: manual\n    issuance_channel: MGID dashboard (self-serve UI)\n    token_endpoint: null\n    token_endpoint_note: >-\n      No machine-readable token/credential-exchange endpoint is documented on any\n      of the three reference pages. Tokens are copied out of the dashboard by a\n      human; there is no documented programmatic rotation, refresh or revocation\n      call.\n    rotation_documented: false\n    expiry_documented: false\n    scopes: []\n    applies_to:\n      - mgid:mgid-advertiser-api\n      - mgid:mgid-publisher-api\n      - mgid:mgid-agency-api\n    sources:\n      - https://help.mgid.com/api-advertisers/\n      - https://help.mgid.com/api-publishers\n      - https://help.mgid.com/api-ra\n\
  transport:\n  https_required: true\n  https_required_evidence: >-\n    \"all API requests must be performed via HTTPS\" — stated on the advertiser and\n    agency reference pages.\nidentity_model:\n  note: >-\n    Authorization is bound to path identifiers rather than to token scopes. Every\n    resource path carries the account identity — {client_id} (advertiser),\n    {authId}/{clientId} (publisher) and {accountId} (agency) — and the token is\n    expected to be entitled to that account. There is no scope, permission or\n    role vocabulary published.\n  path_identifiers:\n    - name: client_id\n      surface: advertiser\n      example_path: /v1/goodhits/clients/{client_id}/campaigns\n    - name: authId\n      surface: publisher\n      example_path: /v1/publishers/{authId}/widget-custom-report\n    - name: clientId\n      surface: publisher\n      example_path: /v2/pub/account/{clientId}/website-custom-report\n    - name: accountId\n      surface: agency\n      example_path: /v1/agencies/{accountId}/clients\n\
  failure_modes:\n  - status: 401\n    body: '{\"errors\":\"Authentication token is missing\"}'\n    observed: true\n    observed_url: https://api.mgid.com/v1/\n    observed_date: '2026-08-12'\n  - status: 401\n    message: invalid token\n    surface: agency\n    source: https://help.mgid.com/api-ra\ngaps:\n  - No OAuth 2.0, OpenID Connect or mTLS surface is published.\n  - No scope or permission model is published, so least-privilege delegation is not expressible.\n  - No documented token lifetime, rotation or revocation endpoint.\n  - Token issuance is UI-only; an agent cannot provision credentials programmatically.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mgid/refs/heads/main/authentication/mgid-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Native Advertising
- Ad Tech
- Publishers
- Advertisers
- Campaigns
- Content Monetization
- Programmatic
---
