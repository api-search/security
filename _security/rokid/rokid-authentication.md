---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Rokid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rokid declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Rokid
provider_slug: rokid
scheme_count: 0
schemes: []
slug: rokid-authentication
source_filename: rokid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://x-docs.rokid.com/docs/en/openapi/ApiKey.html\ndocs: https://x-docs.rokid.com/docs/en/openapi/ApiKey.html\nnotes: >-\n  Derived nothing from an OpenAPI — Rokid publishes no machine-readable spec.\n  Every field below was read from the provider's own published API-key page and\n  request examples, and the unauthenticated failure mode was confirmed by a live\n  probe against api.rokid.com.\napis:\n- name: Rokid Sprite Enterprise OpenAPI\n  base_url: https://api.rokid.com\n  security_schemes:\n  - id: apiKeyBearer\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer <API_KEY>'\n    description: >-\n      A long-lived enterprise API key presented as an HTTP bearer credential.\n      It is not an OAuth access token — there is no token endpoint, no refresh\n      flow and no scope parameter.\n    required_headers:\n      Content-Type: application/json\n    issuance:\n      self_service:\
  \ false\n      process: >-\n        Contact the Rokid sales/business team for OA approval to obtain an\n        enterprise account and API key. There is no developer-portal signup that\n        mints a key.\n      console: https://x-inspection.rokid.com/main/devices\n    lifetime:\n      default_validity: 1 month\n      configurable_at_provisioning: true\n      revocation: >-\n        Keys become invalid if the enterprise account is deregistered. No\n        self-service rotation endpoint is documented.\n    published_guidance:\n    - Prefer one key per app or service to limit blast radius if a key leaks.\n    scopes: none\n    note_on_scopes: >-\n      No scope, permission or role model is documented. A key is all-or-nothing\n      across the device, message, agent, remote-collaboration and AI-work-assistant\n      endpoint families.\n  unauthenticated_behavior:\n    http_status: 200\n    body: '{\"code\":50001,\"message\":\"Authorization 不能为空\",\"success\":false}'\n    note: >-\n   \
  \   A missing Authorization header returns HTTP 200 with an in-body error\n      envelope rather than 401. Clients MUST inspect `success`/`code`, not the\n      HTTP status. See errors/rokid-error-codes.yml.\n    evidence:\n      url: https://api.rokid.com/ar/core/openapi/device/list\n      method: POST\n      http_status: 200\n      fetched: '2026-08-05'\n  gateway_probe:\n    host: openapi.rokid.com\n    result: >-\n      A second API host exists at openapi.rokid.com. Every path — including\n      /openapi.json and /.well-known/* — returns HTTP 401 application/json\n      (\"没有权限\" / no permission) from a Spring-style error envelope. Nothing\n      anonymous is served from it.\n    evidence:\n      url: https://openapi.rokid.com/\n      http_status: 401\n      fetched: '2026-08-05'\n- name: Rokid Global Store — customer accounts (OIDC)\n  base_url: https://global.rokid.com\n  security_schemes:\n  - id: shopifyCustomerAccounts\n    type: openIdConnect\n    openIdConnectUrl: https://global.rokid.com/.well-known/openid-configuration\n\
  \    issuer: https://shopify.com/authentication/62856364211\n    authorization_endpoint: https://shopify.com/authentication/62856364211/oauth/authorize\n    token_endpoint: https://shopify.com/authentication/62856364211/oauth/token\n    jwks_uri: https://shopify.com/authentication/62856364211/.well-known/jwks.json\n    grant_types:\n    - authorization_code\n    - refresh_token\n    - urn:ietf:params:oauth:grant-type:jwt-bearer\n    pkce: S256\n    token_endpoint_auth_methods:\n    - client_secret_basic\n    id_token_signing_alg:\n    - RS256\n    scopes:\n    - openid\n    - email\n    - customer-account-api:full\n    - customer-account-mcp-api:full\n    note: >-\n      This is the Shopify Customer Accounts issuer behind Rokid's global\n      storefront, discovered anonymously at the well-known path. It governs\n      shopper identity on global.rokid.com, NOT the enterprise developer API.\n    evidence:\n      url: https://global.rokid.com/.well-known/openid-configuration\n      http_status:\
  \ 200\n      fetched: '2026-08-05'\nmutual_tls: not documented\napi_key_in_query: not supported\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rokid/refs/heads/main/authentication/rokid-authentication.yml
summary_line: 0 schemes
tags:
- Smart Glasses
- Augmented Reality
- Wearables
- Artificial Intelligence
- Spatial Computing
- Device Management
- Consumer Electronics
- Voice
- Enterprise
- Hardware
- Agents
---
