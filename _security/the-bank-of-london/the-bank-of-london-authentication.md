---
api_key_in: []
api_specs:
- filename: the-bank-of-london-api-openapi.json
  format: json
  label: Bank of London API
  slug: bank-of-london-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-bank-of-london/refs/heads/main/openapi/the-bank-of-london-api-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: The Bank Of London Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Bank of London declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: The Bank of London
provider_slug: the-bank-of-london
scheme_count: 1
schemes:
- algorithm: PS256
  algorithms_supported:
  - PS256
  header: x-jws-signature
  id: jws-message-signature
  jose_header:
    alg: PS256 (only PS256 is supported)
    kid: Key ID indicating which key was used to secure the JWS
  jws_payload_claims:
  - description: The request path per RFC 9110 HTTP Semantics, e.g. /v2/accounts
    name: request-target
  - description: HTTP verb; a mismatch against the actual request method is rejected
    name: method
  - description: Request content-type, e.g. application/json. Omitted when the request has no body.
    name: content-type
  - description: SHA-256 hash of the request body with no whitespace or indentation before hashing
    name: content-digest
  - description: Random unique string per signature to prevent replay. The same nonce must not be reused within a five-minute interval or the request is rejected.
    name: nonce
  - description: Creation time as an integer UNIX timestamp. Only messages signed within the last 5 minutes are accepted.
    name: created
  key_material: API Key + secret pair generated per App in the Developer Studio; the secret is shown once and cannot be retrieved again. Each key is bound permanently to exactly one environment (Live or Sandbox) at creation time.
  location: header
  type: http-message-signature
  verification_steps:
  - The request must be signed by the caller's private key.
  - The signed request must not be more than 5 minutes old.
  - The nonce must be unique — the same request cannot be sent twice.
  - The API Key must be active (not disabled or expired).
  - The message signature must be valid over content, date and authentication of the request.
slug: the-bank-of-london-authentication
source_filename: the-bank-of-london-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: >-\n  https://developer.bankoflondon.com/docs/overviews/authentication-message-signature-guide +\n  https://developer.bankoflondon.com/docs/overviews/architecture-security-guide +\n  https://developer.bankoflondon.com/docs/guides/getting-started-guide +\n  openapi/the-bank-of-london-api-openapi.json (components.parameters.JwsSignature)\nsummary: >-\n  The Bank of London API does not use bearer tokens or a plain API-key header. Every request carries\n  a detached JSON Web Signature in the `x-jws-signature` header, produced with the private key of an\n  API key pair created inside the Developer Studio. The signature binds the request target, method,\n  content-type, a SHA-256 content digest, a single-use nonce and a creation timestamp, so a captured\n  request cannot be replayed or altered. The published OpenAPI declares NO `components.securitySchemes`\n  block at all — the scheme is carried only as a required header parameter\
  \ (`JwsSignature`) applied to\n  all 58 operations, which is why a spec-only reader would wrongly conclude this API is unauthenticated.\nspec_declared:\n  security_schemes: {}\n  note: >-\n    components.securitySchemes is an empty object in the published contract, and there is no top-level\n    `security` array. This is a real gap in the contract, not in the product: the header parameter\n    `x-jws-signature` ($ref components/parameters/JwsSignature) is marked required on every operation.\nschemes:\n- id: jws-message-signature\n  type: http-message-signature\n  location: header\n  header: x-jws-signature\n  algorithm: PS256\n  algorithms_supported: [PS256]\n  key_material: >-\n    API Key + secret pair generated per App in the Developer Studio; the secret is shown once and\n    cannot be retrieved again. Each key is bound permanently to exactly one environment (Live or\n    Sandbox) at creation time.\n  jose_header:\n    alg: PS256 (only PS256 is supported)\n    kid: Key ID indicating\
  \ which key was used to secure the JWS\n  jws_payload_claims:\n  - name: request-target\n    description: The request path per RFC 9110 HTTP Semantics, e.g. /v2/accounts\n  - name: method\n    description: HTTP verb; a mismatch against the actual request method is rejected\n  - name: content-type\n    description: Request content-type, e.g. application/json. Omitted when the request has no body.\n  - name: content-digest\n    description: SHA-256 hash of the request body with no whitespace or indentation before hashing\n  - name: nonce\n    description: >-\n      Random unique string per signature to prevent replay. The same nonce must not be reused within\n      a five-minute interval or the request is rejected.\n  - name: created\n    description: >-\n      Creation time as an integer UNIX timestamp. Only messages signed within the last 5 minutes are\n      accepted.\n  verification_steps:\n  - The request must be signed by the caller's private key.\n  - The signed request must not be\
  \ more than 5 minutes old.\n  - The nonce must be unique — the same request cannot be sent twice.\n  - The API Key must be active (not disabled or expired).\n  - The message signature must be valid over content, date and authentication of the request.\noauth2:\n  present_on_main_api: false\n  note: >-\n    No OAuth 2.0 or OpenID Connect flow exists on the Bank of London API v2. OAuth/OIDC applies only\n    to the separate PSD2 / Open Banking UK v3.1 TPP interface operated by Salt Edge Priora, where\n    TPPs perform dynamic client registration and PSU consent via OIDC. That interface is documented\n    at https://priora.saltedge.com/docs/open_banking/tbol/v3.1 and no scope reference is published by\n    either party, so no scopes/ artifact is emitted for this provider.\nportal_authentication:\n  mfa_required: true\n  note: >-\n    Mandatory two-factor authentication for all Developer Studio users, enforced strong password\n    policy, role-based team access with audit logs covering API\
  \ key creation/approval, invitations\n    and role changes.\nkey_handling_guidance:\n  source: https://developer.bankoflondon.com/docs/overviews/architecture-security-guide\n  recommendations:\n  - Store keys in an industry-recognised secrets vault (AWS Secrets Manager, HashiCorp Vault, GCP, Azure).\n  - Never place keys in plaintext, source code, logs or email.\n  - Do not let end users contact the API directly; proxy through a gateway in your own secure data centre.\ntransport:\n  tls_minimum: TLSv1.2\n  note: All Bank of London services are accessible only over SSL with non-downgradable TLS 1.2 or higher.\ndocs:\n- https://developer.bankoflondon.com/docs/overviews/authentication-message-signature-guide\n- https://developer.bankoflondon.com/docs/overviews/architecture-security-guide\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-bank-of-london/refs/heads/main/authentication/the-bank-of-london-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Banking
- Clearing Bank
- Payments
- Banking as a Service
- Embedded Finance
- Open Banking
- PSD2
- Faster Payments
- Financial-Services
- United Kingdom
- Virtual Accounts
---
