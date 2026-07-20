---
api_key_in:
- header
api_specs:
- filename: appcharge-openapi.yml
  format: yaml
  label: Appcharge Publisher API
  slug: appcharge-publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-openapi.yml
auth_types:
- apiKey
- oauth2
- mutualTLS
- hmac-signature
description: 'Appcharge uses three distinct authentication surfaces: (1) the publisher REST API authenticates with the x-publisher-token API key header (from the Publisher Dashboard > Settings > Integration); (2) webhooks and Appcharge-> publisher callbacks are verified with an HMAC-SHA256 signature over "{timestamp}.{json_payload}" carried in the `signature: t=...,v1=...` header (plus x-publisher-token and x-project-id), with a ~5-minute replay window; (3) the hosted MCP server is protected by OAuth 2.0 (authorization_code + PKCE). mTLS is supported for sensitive server-to-server integrations.'
kind: authentication
layout: security
method: searched
name: Appcharge Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Appcharge secures its APIs with apiKey, oauth2, mutualTLS, and hmac-signature across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Appcharge
provider_slug: appcharge
scheme_count: 4
schemes:
- description: Publisher token from the Publisher Dashboard (Settings > Integration). Required on all REST API calls. Can be shared across multiple Appcharge accounts.
  in: header
  name: PublisherTokenAuth
  parameter: x-publisher-token
  sources:
  - openapi/appcharge-openapi.yml
  type: apiKey
- algorithm: HMAC-SHA256
  also_sent:
  - x-publisher-token
  - x-project-id
  description: Signature Appcharge attaches to every outbound webhook/callback so the publisher can verify authenticity and integrity. Timestamp is a Unix ms value; publishers reconstruct the HMAC with their main key (Settings > Integration) and compare.
  format: t={timestamp},v1={hex_signature}
  header: signature
  input: '{timestamp}.{json_payload}'
  name: WebhookSignature
  replay_window: ~5 minutes
  sources:
  - https://docs.appcharge.com/api-reference/events/v2/introduction
  type: hmac
- applies_to: hosted MCP server (mcp.appcharge.com)
  authorizationUrl: https://api.appcharge.com/oauth/authorize
  flow: authorizationCode
  name: OAuth2
  scopes:
  - mcp:read
  - mcp:write
  sources:
  - https://api.appcharge.com/.well-known/oauth-authorization-server
  tokenUrl: https://api.appcharge.com/oauth/token
  type: oauth2
- description: mTLS supported for server-to-server integrations that require both parties to present and verify certificates.
  name: MutualTLS
  sources:
  - https://docs.appcharge.com/merchant-of-record/security/about-security-at-appcharge
  type: mutualTLS
slug: appcharge-authentication
source_filename: appcharge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/appcharge-openapi.yml + https://docs.appcharge.com/api-reference/appcharge-publisher-secure-communication + https://docs.appcharge.com/merchant-of-record/security/about-security-at-appcharge\ndocs: https://docs.appcharge.com/api-reference/appcharge-publisher-secure-communication\ndescription: >-\n  Appcharge uses three distinct authentication surfaces: (1) the publisher REST\n  API authenticates with the x-publisher-token API key header (from the\n  Publisher Dashboard > Settings > Integration); (2) webhooks and Appcharge->\n  publisher callbacks are verified with an HMAC-SHA256 signature over\n  \"{timestamp}.{json_payload}\" carried in the `signature: t=...,v1=...` header\n  (plus x-publisher-token and x-project-id), with a ~5-minute replay window;\n  (3) the hosted MCP server is protected by OAuth 2.0 (authorization_code +\n  PKCE). mTLS is supported for sensitive server-to-server integrations.\nsummary:\n  types:\
  \ [apiKey, oauth2, mutualTLS, hmac-signature]\n  api_key_in: [header]\n  api_key_names: [x-publisher-token]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: PublisherTokenAuth\n    type: apiKey\n    in: header\n    parameter: x-publisher-token\n    description: >-\n      Publisher token from the Publisher Dashboard (Settings > Integration).\n      Required on all REST API calls. Can be shared across multiple Appcharge\n      accounts.\n    sources: [openapi/appcharge-openapi.yml]\n  - name: WebhookSignature\n    type: hmac\n    algorithm: HMAC-SHA256\n    header: signature\n    format: t={timestamp},v1={hex_signature}\n    input: \"{timestamp}.{json_payload}\"\n    replay_window: ~5 minutes\n    also_sent: [x-publisher-token, x-project-id]\n    description: >-\n      Signature Appcharge attaches to every outbound webhook/callback so the\n      publisher can verify authenticity and integrity. Timestamp is a Unix ms\n      value; publishers reconstruct the HMAC with their main key\
  \ (Settings >\n      Integration) and compare.\n    sources: [https://docs.appcharge.com/api-reference/events/v2/introduction]\n  - name: OAuth2\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://api.appcharge.com/oauth/authorize\n    tokenUrl: https://api.appcharge.com/oauth/token\n    scopes: [mcp:read, mcp:write]\n    applies_to: hosted MCP server (mcp.appcharge.com)\n    sources: [https://api.appcharge.com/.well-known/oauth-authorization-server]\n  - name: MutualTLS\n    type: mutualTLS\n    description: >-\n      mTLS supported for server-to-server integrations that require both parties\n      to present and verify certificates.\n    sources: [https://docs.appcharge.com/merchant-of-record/security/about-security-at-appcharge]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/authentication/appcharge-authentication.yml
summary_line: apiKey/oauth2/mutualTLS/hmac-signature · 4 schemes
tags:
- Company
- Payments
- Monetization
- Merchant of Record
- Mobile Games
- Gaming
- Checkout
- In-Game Purchases
- Web Store
- eCommerce
---
