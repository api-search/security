---
anonymous_access: false
api_key_in:
- path
api_specs:
- filename: level2-hub-controller-openapi.json
  format: json
  label: Level2 Hub API
  slug: level2-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-hub-controller-openapi.json
- filename: level2-backtesting-api-openapi.yml
  format: yaml
  label: level2 Backtesting API
  slug: level2-backtesting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-backtesting-api-openapi.yml
- filename: level2-discovery-api-openapi.yml
  format: yaml
  label: level2 Discovery API
  slug: level2-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-discovery-api-openapi.yml
- filename: level2-market-data-api-openapi.yml
  format: yaml
  label: level2 Market Data API
  slug: level2-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-market-data-api-openapi.yml
- filename: level2-strategies-api-openapi.yml
  format: yaml
  label: level2 Strategies API
  slug: level2-strategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-strategies-api-openapi.yml
- filename: level2-technical-analysis-api-openapi.yml
  format: yaml
  label: level2 Technical Analysis API
  slug: level2-technical-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-technical-analysis-api-openapi.yml
- filename: level2-users-api-openapi.yml
  format: yaml
  label: level2 Users API
  slug: level2-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-users-api-openapi.yml
auth_types:
- http
- apiKey
description: Authentication across the Level2 API surface. The live Broker API is protected by a bearer JWT the broker partner mints itself; the legacy Bytemine signal API used an API key embedded in the URL PATH. The live contract at https://hub2.trylevel2.com/openapi.json declares no securitySchemes at all, so the model below is read from the provider's documentation and from the headers in its own published Postman collection rather than from the spec.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Level2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Level2 secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Level2
provider_slug: level2
scheme_count: 2
schemes:
- bearerFormat: JWT
  credential_issuance: Out of band. The signing secret and the `domain` value are, in the provider's words, "to be shared separately"; API access itself is requested by emailing contact@trylevel2.com.
  description: The broker partner generates an HS256 JSON Web Token itself, signing it with a secret Level2 shares out of band. The payload carries a `domain` claim (the partner's Level2 subdomain, e.g. antostrategy.trylevel2.com in the provider's own worked example) and a `token_expiry` claim.
  evidence:
  - https://learn.trylevel2.com/docs/Broker/API/authentication
  - https://learn.trylevel2.com/docs/Broker/API/broker-api
  - 'https://learn.trylevel2.com/broker_apis.json (every request sends Authorization: Bearer [token])'
  name: bearerAuth
  scheme: bearer
  self_service: false
  sources:
  - https://learn.trylevel2.com/docs/Broker/API/authentication
  status: current
  surface: Level2 Hub / Broker API (https://hub2.trylevel2.com)
  token_lifetime:
    enforcement: '"Tokens exceeding 180 minutes of validity will be automatically invalidated by the system. Upon automatic expiration, a new JWT with a 180-minute token_expiry must be generated."'
    maximum_minutes: 180
    recommended_minutes: 180
  type: http
- caution: A credential in the path is logged by every proxy, CDN and browser history along the way. It is recorded here because the provider documents it, not because it is recommended.
  description: An API key interpolated directly into the request PATH — e.g. /checkForCandlestick/{api_key}/TSLA/5m. The Bytemine documentation obtains the key from a developer portal at https://app.bytemine.io/developers.
  in: path
  liveness:
    checked: '2026-09-17'
    note: app.bytemine.io does not resolve (NXDOMAIN), so the documented key-issuance portal is unreachable; valhalla.bytemine.workers.dev resolves but returns HTTP 500 "Wrong Api Call" on every path.
  name: apiKeyPath
  parameter: api_key
  sources:
  - https://guide.bytemine.io/technical-documentation/api-documentation.md
  - openapi/_original/level2-strategy-builder-openapi.yml
  status: legacy
  surface: Legacy Bytemine signal API (app.bytemine.io/api, valhalla.bytemine.workers.dev)
  type: apiKey
slug: level2-authentication
source_filename: level2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  https://learn.trylevel2.com/docs/Broker/API/authentication;\n  https://learn.trylevel2.com/docs/Broker/API/broker-api;\n  https://learn.trylevel2.com/broker_apis.json (provider-published Postman collection);\n  https://guide.bytemine.io/technical-documentation/api-documentation.md;\n  openapi/level2-hub-controller-openapi.json;\n  openapi/_original/level2-strategy-builder-openapi.yml;\n  openapi/_original/level2-tradestation-integration-openapi.yml\ndocs: https://learn.trylevel2.com/docs/Broker/API/authentication\ndescription: >-\n  Authentication across the Level2 API surface. The live Broker API is protected by a bearer JWT the\n  broker partner mints itself; the legacy Bytemine signal API used an API key embedded in the URL\n  PATH. The live contract at https://hub2.trylevel2.com/openapi.json declares no securitySchemes at\n  all, so the model below is read from the provider's documentation and from the headers in\
  \ its own\n  published Postman collection rather than from the spec.\nsummary:\n  types:\n    - http\n    - apiKey\n  api_key_in:\n    - path\n  spec_declares_security: false\n  spec_declares_security_note: >-\n    The FastAPI-generated contract carries no components.securitySchemes block and no top-level\n    security requirement, even though every /broker/* operation requires a bearer token in practice.\n    overlays/level2-hub-controller-overlay.yaml adds the documented scheme without mutating the\n    original.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    surface: Level2 Hub / Broker API (https://hub2.trylevel2.com)\n    status: current\n    description: >-\n      The broker partner generates an HS256 JSON Web Token itself, signing it with a secret Level2\n      shares out of band. The payload carries a `domain` claim (the partner's Level2 subdomain, e.g.\n      antostrategy.trylevel2.com in the provider's own worked example) and a\
  \ `token_expiry` claim.\n    token_lifetime:\n      recommended_minutes: 180\n      maximum_minutes: 180\n      enforcement: >-\n        \"Tokens exceeding 180 minutes of validity will be automatically invalidated by the system.\n        Upon automatic expiration, a new JWT with a 180-minute token_expiry must be generated.\"\n    self_service: false\n    credential_issuance: >-\n      Out of band. The signing secret and the `domain` value are, in the provider's words, \"to be\n      shared separately\"; API access itself is requested by emailing contact@trylevel2.com.\n    evidence:\n      - https://learn.trylevel2.com/docs/Broker/API/authentication\n      - https://learn.trylevel2.com/docs/Broker/API/broker-api\n      - 'https://learn.trylevel2.com/broker_apis.json (every request sends Authorization: Bearer [token])'\n    sources:\n      - https://learn.trylevel2.com/docs/Broker/API/authentication\n  - name: apiKeyPath\n    type: apiKey\n    in: path\n    parameter: api_key\n    surface:\
  \ Legacy Bytemine signal API (app.bytemine.io/api, valhalla.bytemine.workers.dev)\n    status: legacy\n    description: >-\n      An API key interpolated directly into the request PATH — e.g.\n      /checkForCandlestick/{api_key}/TSLA/5m. The Bytemine documentation obtains the key from a\n      developer portal at https://app.bytemine.io/developers.\n    caution: >-\n      A credential in the path is logged by every proxy, CDN and browser history along the way. It is\n      recorded here because the provider documents it, not because it is recommended.\n    liveness:\n      checked: '2026-09-17'\n      note: >-\n        app.bytemine.io does not resolve (NXDOMAIN), so the documented key-issuance portal is\n        unreachable; valhalla.bytemine.workers.dev resolves but returns HTTP 500 \"Wrong Api Call\" on\n        every path.\n    sources:\n      - https://guide.bytemine.io/technical-documentation/api-documentation.md\n      - openapi/_original/level2-strategy-builder-openapi.yml\noauth:\n\
  \  as_server: false\n  as_client: true\n  note: >-\n    Level2 publishes no authorization server (/.well-known/oauth-authorization-server is 404 on every\n    host). It is an OAuth CLIENT of the brokers it connects to: the contract carries\n    /broker-oauth/public/callback, /broker-oauth/connecttrade/callback, /broker-oauth/sterling and\n    /ctrader_access + /ctrader_auth_callback. End users may additionally sign in with Google\n    (POST /auth/google), but no OIDC discovery document is served.\nend_user_auth:\n  methods:\n    - email + password (POST /login, POST /register_user)\n    - Google sign-in (POST /auth/google)\n    - email OTP (POST /generate_email_otp, POST /verify_otp_token)\n    - SMS OTP (POST /send_sms_otp, POST /validate_sms_otp)\n  note: Platform sign-in for traders, distinct from the partner-facing Broker API token above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/authentication/level2-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Trading
- Fintech
- Financial-Services
- Automation
- No-Code
- Backtesting
- Strategies
- Brokerage
- Market Data
- Prediction Markets
---
