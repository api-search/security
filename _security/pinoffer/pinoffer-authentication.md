---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Pinoffer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pinoffer declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Pinoffer
provider_slug: pinoffer
scheme_count: 5
schemes:
- applies_to: Store Connector API (the endpoints a merchant implements for Convertedin to poll)
  description: '"Use your token provided inside converted.in after on boarding process to authenticate the request using form-data body." A fixed, non-expiring token issued at onboarding, sent as a form field rather than a header.'
  encoding: multipart/form-data
  expiry_documented: false
  id: store-connector-token
  in: body
  issued_by: Convertedin platform, at onboarding
  parameter: token
  rotation_documented: false
  source: https://developer.converted.in/api-1/categories.md
  type: apiKey
  weaknesses:
  - A credential carried in a form-data body is not covered by standard header redaction and will be written to request logs and proxy traces by default.
  - No documented rotation, expiry, revocation or scoping.
- applies_to: Webhook ingest API (https://app.converted.in/api/webhooks/api/)
  companion_header: X-Shop-Domain
  description: Fixed token header, paired with a mandatory `X-Shop-Domain` header identifying the sending store. Not a signature — the payload is not signed or hashed, so a receiver cannot verify integrity or replay-protect a delivery.
  expiry_documented: false
  id: webhook-token
  in: header
  parameter: token
  rotation_documented: false
  source: https://developer.converted.in/api-1/webhooks.md
  type: apiKey
  x-evidence:
    body: '{"msg":"please send in header [x-shop-domain]"}'
    http_status: 401
    method: POST
    note: Auth enforcement observed live on an anonymous request.
    probed: '2026-08-12'
    url: https://app.converted.in/api/webhooks/api/orders/create
- applies_to: Loyalty & POS Integration API (the endpoints a POS/loyalty vendor implements)
  description: 'Custom `Access-Token: {access_token}` header on every GET. Not RFC 6750 Bearer — a non-standard header name, so off-the-shelf HTTP clients and agent runtimes will not populate it from a standard credential store.'
  expiry_documented: false
  id: loyalty-pos-access-token
  in: header
  parameter: Access-Token
  rotation_documented: false
  source: https://developer.converted.in/loyalty-and-pos-integration/store-info.md
  type: apiKey
- applies_to: Convertedin Pixel / Client SDK (browser)
  description: '`ciq("init", "{your-pixel-key-goes-here}")`. A public, browser-visible identifier by design — an analytics write key, not a secret. Treat as public.'
  id: pixel-key
  in: client-side-init
  parameter: pixel key
  public_by_design: true
  source: https://developer.converted.in/pixel/client-sdk.md
  type: apiKey
- applies_to: Convertedin DSP / Flyerz Web SDK (embedded iframe)
  description: '`https://app-flyerz.converted.in/?token=x` — a portal-config token placed in an iframe `src` query string. The docs say "The token refereed to your portal config, please ask for that", i.e. it is issued by hand, not self-service.'
  id: dsp-iframe-token
  in: query
  parameter: token
  rotation_documented: false
  source: https://developer.converted.in/dsp/getting-started.md
  type: apiKey
  weaknesses:
  - A credential in a URL query string leaks through Referer headers, browser history and server access logs.
slug: pinoffer-authentication
source_filename: pinoffer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://developer.converted.in/api-1/getting-started.md,\n  https://developer.converted.in/api-1/categories.md,\n  https://developer.converted.in/api-1/webhooks.md,\n  https://developer.converted.in/loyalty-and-pos-integration/store-info.md,\n  https://developer.converted.in/pixel/client-sdk.md,\n  https://developer.converted.in/dsp/getting-started.md\nnote: >-\n  Derived by reading the docs, NOT from an OpenAPI document — Convertedin publishes\n  no machine-readable spec, so there are no `securitySchemes` to parse. Every scheme\n  below is quoted from a published documentation page. All four are static shared\n  secrets; Convertedin publishes no OAuth 2.0, OpenID Connect or mTLS surface, so\n  `scopes/` is intentionally absent rather than empty.\ndocs: https://developer.converted.in/api-1/getting-started\nmodel: static-shared-secret\noauth2: false\nopenid_connect: false\nmutual_tls: false\nschemes:\n- id: store-connector-token\n\
  \  applies_to: Store Connector API (the endpoints a merchant implements for Convertedin to poll)\n  type: apiKey\n  in: body\n  parameter: token\n  encoding: multipart/form-data\n  description: >-\n    \"Use your token provided inside converted.in after on boarding process to\n    authenticate the request using form-data body.\" A fixed, non-expiring token\n    issued at onboarding, sent as a form field rather than a header.\n  issued_by: Convertedin platform, at onboarding\n  rotation_documented: false\n  expiry_documented: false\n  source: https://developer.converted.in/api-1/categories.md\n  weaknesses:\n  - >-\n    A credential carried in a form-data body is not covered by standard header\n    redaction and will be written to request logs and proxy traces by default.\n  - No documented rotation, expiry, revocation or scoping.\n- id: webhook-token\n  applies_to: Webhook ingest API (https://app.converted.in/api/webhooks/api/)\n  type: apiKey\n  in: header\n  parameter: token\n  description:\
  \ >-\n    Fixed token header, paired with a mandatory `X-Shop-Domain` header identifying\n    the sending store. Not a signature — the payload is not signed or hashed, so a\n    receiver cannot verify integrity or replay-protect a delivery.\n  companion_header: X-Shop-Domain\n  rotation_documented: false\n  expiry_documented: false\n  source: https://developer.converted.in/api-1/webhooks.md\n  x-evidence:\n    probed: '2026-08-12'\n    url: https://app.converted.in/api/webhooks/api/orders/create\n    method: POST\n    http_status: 401\n    body: '{\"msg\":\"please send in header [x-shop-domain]\"}'\n    note: Auth enforcement observed live on an anonymous request.\n- id: loyalty-pos-access-token\n  applies_to: Loyalty & POS Integration API (the endpoints a POS/loyalty vendor implements)\n  type: apiKey\n  in: header\n  parameter: Access-Token\n  description: >-\n    Custom `Access-Token: {access_token}` header on every GET. Not RFC 6750\n    Bearer — a non-standard header name, so off-the-shelf\
  \ HTTP clients and agent\n    runtimes will not populate it from a standard credential store.\n  rotation_documented: false\n  expiry_documented: false\n  source: https://developer.converted.in/loyalty-and-pos-integration/store-info.md\n- id: pixel-key\n  applies_to: Convertedin Pixel / Client SDK (browser)\n  type: apiKey\n  in: client-side-init\n  parameter: pixel key\n  description: >-\n    `ciq(\"init\", \"{your-pixel-key-goes-here}\")`. A public, browser-visible\n    identifier by design — an analytics write key, not a secret. Treat as public.\n  public_by_design: true\n  source: https://developer.converted.in/pixel/client-sdk.md\n- id: dsp-iframe-token\n  applies_to: Convertedin DSP / Flyerz Web SDK (embedded iframe)\n  type: apiKey\n  in: query\n  parameter: token\n  description: >-\n    `https://app-flyerz.converted.in/?token=x` — a portal-config token placed in\n    an iframe `src` query string. The docs say \"The token refereed to your portal\n    config, please ask for that\"\
  , i.e. it is issued by hand, not self-service.\n  rotation_documented: false\n  source: https://developer.converted.in/dsp/getting-started.md\n  weaknesses:\n  - >-\n    A credential in a URL query string leaks through Referer headers, browser\n    history and server access logs.\nend_user_auth:\n  description: >-\n    The Flyerz DSP web SDK authenticates END USERS separately with a phone number\n    plus a one-time password (OTP) delivered by SMS, then links a Facebook ad\n    account. This is a product login flow, not an API credential.\n  source: https://developer.converted.in/dsp/getting-started.md\ngaps:\n- no OAuth 2.0 / OIDC surface, therefore no scopes and no delegated access\n- no documented token rotation, expiry, or revocation for any scheme\n- no signature verification on webhook deliveries\n- no self-service credential issuance — every token is handed out at onboarding\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinoffer/refs/heads/main/authentication/pinoffer-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Advertising Technology
- Marketing Technology
- E-commerce
- Marketing Automation
- Customer Data
- Lead Generation
- Payments
- Emerging Markets
- MENA
- Advertising
- Webhooks
---
