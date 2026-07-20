---
api_key_in: []
auth_types: []
description: Lalamove Delivery API v3 authenticates every request with an HMAC SHA256 request signature rather than a bearer token or OAuth flow. Credentials are a paired API KEY and API SECRET issued per market through the Partner Portal. Because the signature covers the timestamp, method, path and body, credentials are never transmitted in a replayable form and there is no token endpoint, refresh flow, or scope surface.
kind: authentication
layout: security
method: searched
name: Lalamove Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lalamove declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lalamove
provider_slug: lalamove
scheme_count: 1
schemes:
- example: hmac pk_test_key:1545880607433:5133946c6a0ba259...
  format: hmac {KEY}:{TIMESTAMP}:{SIGNATURE}
  header: Authorization
  id: hmac-sha256
  in: header
  scheme: hmac
  signing:
    algorithm: HMAC-SHA256
    encoding: lowercase hexadecimal (base 16)
    raw_signature_template: '{TIMESTAMP}\r\n{HTTP_METHOD}\r\n{PATH}\r\n\r\n{BODY}'
    secret: API SECRET
    steps:
    - Generate a Unix timestamp in milliseconds (e.g. 1545880607433).
    - Build the raw signature string {TIMESTAMP}\r\n{METHOD}\r\n{PATH}\r\n\r\n{BODY}. For GET requests the body segment is omitted.
    - Compute HmacSHA256(rawSignature, API_SECRET).
    - Render the digest as lowercase hex.
    - Assemble the Authorization header as hmac {API_KEY}:{TIMESTAMP}:{SIGNATURE}. The timestamp in the header MUST match the timestamp used to build the signature.
  type: http
slug: lalamove-authentication
source_filename: lalamove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.lalamove.com/ (Authentication section)\ndescription: >-\n  Lalamove Delivery API v3 authenticates every request with an HMAC SHA256\n  request signature rather than a bearer token or OAuth flow. Credentials are a\n  paired API KEY and API SECRET issued per market through the Partner Portal.\n  Because the signature covers the timestamp, method, path and body, credentials\n  are never transmitted in a replayable form and there is no token endpoint,\n  refresh flow, or scope surface.\nbase_urls:\n  production: https://rest.lalamove.com/v3\n  sandbox: https://rest.sandbox.lalamove.com/v3\ntransport:\n  https_required: true\n  note: All requests must use HTTPS; plain HTTP calls fail.\nschemes:\n  - id: hmac-sha256\n    type: http\n    scheme: hmac\n    in: header\n    header: Authorization\n    format: \"hmac {KEY}:{TIMESTAMP}:{SIGNATURE}\"\n    example: \"hmac pk_test_key:1545880607433:5133946c6a0ba259...\"\n\
  \    signing:\n      algorithm: HMAC-SHA256\n      encoding: lowercase hexadecimal (base 16)\n      secret: API SECRET\n      raw_signature_template: \"{TIMESTAMP}\\\\r\\\\n{HTTP_METHOD}\\\\r\\\\n{PATH}\\\\r\\\\n\\\\r\\\\n{BODY}\"\n      steps:\n        - Generate a Unix timestamp in milliseconds (e.g. 1545880607433).\n        - >-\n          Build the raw signature string\n          {TIMESTAMP}\\r\\n{METHOD}\\r\\n{PATH}\\r\\n\\r\\n{BODY}. For GET requests the\n          body segment is omitted.\n        - Compute HmacSHA256(rawSignature, API_SECRET).\n        - Render the digest as lowercase hex.\n        - >-\n          Assemble the Authorization header as\n          hmac {API_KEY}:{TIMESTAMP}:{SIGNATURE}. The timestamp in the header\n          MUST match the timestamp used to build the signature.\ncredentials:\n  api_key:\n    sandbox_prefix: pk_test\n    production_prefix: pk_prod\n  api_secret:\n    sandbox_prefix: sk_test\n    production_prefix: sk_prod\n  issuance: https://partnerportal.lalamove.com\
  \ (Developers tab)\n  note: >-\n    Production credentials are released only after the production wallet is\n    topped up. Sandbox credentials require no approval.\nrequired_headers:\n  - name: Authorization\n    required: true\n    description: HMAC credential triplet — hmac {KEY}:{TIMESTAMP}:{SIGNATURE}\n  - name: Market\n    required: true\n    description: >-\n      Target market in UN/LOCODE form (HK, SG, MY, TH, PH, ID, VN, TW, JP, MX,\n      BR). Scopes the request to one market's fleet, pricing and service types.\n  - name: Request-ID\n    required: true\n    description: >-\n      Client-generated nonce/UUID. Used as the request's unique identifier for\n      support and tracing. NOT an idempotency key — the documentation does not\n      describe it as deduplicating or replaying repeated requests.\n  - name: Content-Type\n    required: true\n    description: application/json\noauth2: false\noidc: false\nscopes:\n  supported: false\n  note: >-\n    Key-and-secret HMAC auth has\
  \ no scope or permission surface, so no\n    scopes/ artifact is produced for this provider.\nmtls: false\nwebhook_authentication:\n  note: >-\n    Webhook delivery is configured by URL through PATCH /v3/webhook or the\n    Partner Portal. The public documentation reviewed does not describe a\n    signature header for verifying inbound webhook payloads; consumers should\n    confirm current webhook verification guidance with partner.support@lalamove.com.\ndocs: https://developers.lalamove.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lalamove/refs/heads/main/authentication/lalamove-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Technology
- Logistics
- Delivery
- Last Mile Delivery
- Courier
- Transportation
- On Demand
- Fleet
- Shipping
---
