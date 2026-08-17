---
api_key_in:
- query
- body
api_specs:
- filename: VidyardAnalyticsWebhooks.postman_collection.json
  format: json
  label: Vidyard Analytics Webhook API
  slug: vidyard-analytics-webhook-api
  spec_type: Postman
  url: https://vy-docs.s3.amazonaws.com/postman/VidyardAnalyticsWebhooks.postman_collection.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Vidyard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vidyard secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vidyard
provider_slug: vidyard
scheme_count: 1
schemes:
- applies_to:
  - Vidyard Dashboard API
  - Vidyard Analytics Webhook API
  - Vidyard Video Agent API
  description: 'A static, long-lived Vidyard API token. Passed either as a query parameter on the URL or as an attribute in the JSON request body — the documentation presents both as equally valid.

    '
  example_form: https://api.vidyard.com/endpoint?auth_token={yourToken}
  in: query
  name: auth_token
  parameter: auth_token
  required_headers:
    Accept: application/json
    Content-Type: application/json
  type: apiKey
slug: vidyard-authentication
source_filename: vidyard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >\n  https://knowledge.vidyard.com/hc/en-us/articles/360010000133-How-to-use-the-Vidyard-Dashboard-API\ndocs: https://knowledge.vidyard.com/hc/en-us/articles/360009875814-How-to-access-your-Vidyard-API-tokens\nderivation_note: >\n  Derived by hand from Vidyard's published documentation, not from a spec.\n  0-working/derive-authentication.py was not run because Vidyard publishes no\n  OpenAPI/Swagger document to read securitySchemes from — see\n  conformance/vidyard-conformance.yml.\n\nsummary:\n  types: [apiKey]\n  api_key_in: [query, body]\n  api_key_in_header: false\n  oauth2: false\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  bearer: false\n\nschemes:\n  - name: auth_token\n    type: apiKey\n    in: query\n    parameter: auth_token\n    applies_to:\n      - Vidyard Dashboard API\n      - Vidyard Analytics Webhook API\n      - Vidyard Video Agent API\n    description: >\n      A static, long-lived\
  \ Vidyard API token. Passed either as a query\n      parameter on the URL or as an attribute in the JSON request body — the\n      documentation presents both as equally valid.\n    example_form: https://api.vidyard.com/endpoint?auth_token={yourToken}\n    required_headers:\n      Content-Type: application/json\n      Accept: application/json\n\nscoping:\n  model: folder + role\n  folder_scope: >\n    Tokens are unique to each FOLDER in the account. A token issued in a\n    subfolder can only act on assets in that folder. This is the primary\n    authorization boundary — there is no separate scope or permission parameter\n    on a request; the folder the token came from decides what it can reach.\n  role_scope: >\n    Tokens are also role-based. A token inherits exactly the dashboard actions\n    the issuing user's role permits, so two tokens from the same folder can\n    have different effective capability.\n  issuance:\n    ui_path: Admin > API Tokens\n    required_permission: Edit API\
  \ tokens\n    team_requirement: >\n      The user must belong to a Team with the \"Edit API tokens\" permission\n      enabled. Analytics webhook setup through the UI instead requires the\n      \"Edit Integrations\" permission.\n  note: >\n    Users only see the API tokens relevant to their own role, and must switch\n    folders in the UI (\"Change Folder\") to obtain a token for a different\n    branch of the tree.\n\nrelated_mechanisms:\n  - name: Secure embed JWT\n    type: JWT\n    description: >\n      A separate, viewer-facing mechanism — not API authentication. Signed JSON\n      Web Tokens restrict playback of embedded videos to an authorized site.\n    docs: https://knowledge.vidyard.com/hc/en-us/articles/360009997733-Restrict-Vidyard-videos-to-your-secure-site-using-JSON-Web-Tokens\n  - name: Analytics webhook security_key\n    type: shared secret\n    description: >\n      Inbound-verification secret echoed on webhook delivery so a receiver can\n      confirm the caller is\
  \ Vidyard. Not a request signature.\n    cross_reference: asyncapi/vidyard-webhooks.yml\n\ncommercial_gate:\n  note: >\n    Vidyard's plan documentation states the Dashboard, Video Agent and\n    Analytics Webhook APIs are gated behind the Enterprise tier, while the\n    knowledge-base \"Who Can Use This Feature?\" banners list Free/Starter/Teams/\n    Enterprise with the caveat that the user must hold the Edit API tokens\n    permission. The two published statements disagree; treat API access as\n    sales-gated in practice.\n  see: plans/vidyard-plans-pricing.yml\n\ngaps:\n  - No OAuth 2.0 authorization-code flow — third-party apps cannot obtain delegated user access.\n  - No OpenID Connect discovery document (/.well-known/openid-configuration 404s on every host).\n  - Tokens are accepted in the QUERY STRING, where they leak into server logs, browser history, proxies and Referer headers.\n  - No documented token expiry, rotation, or revocation procedure.\n  - No Authorization header\
  \ support is documented, which is the conventional and safer placement.\n  - No scopes: capability is implied by folder and role, and is not visible or assertable at request time.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidyard/refs/heads/main/authentication/vidyard-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Video
- Video Platform
- Video Analytics
- Video Sharing
- Sales Video
- CRM Integration
- Marketing
- AI Video
- Webhooks
---
