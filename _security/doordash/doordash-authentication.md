---
anonymous_access: false
api_key_in: []
api_specs:
- filename: doordash-addresses-api-openapi.yml
  format: yaml
  label: doordash Addresses API
  slug: doordash-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-addresses-api-openapi.yml
- filename: doordash-businesses-api-openapi.yml
  format: yaml
  label: doordash Businesses API
  slug: doordash-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-businesses-api-openapi.yml
- filename: doordash-catalog-api-openapi.yml
  format: yaml
  label: doordash Catalog API
  slug: doordash-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-catalog-api-openapi.yml
- filename: doordash-deliveries-api-openapi.yml
  format: yaml
  label: doordash Deliveries API
  slug: doordash-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-deliveries-api-openapi.yml
- filename: doordash-inventory-api-openapi.yml
  format: yaml
  label: doordash Inventory API
  slug: doordash-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-inventory-api-openapi.yml
- filename: doordash-items-api-openapi.yml
  format: yaml
  label: doordash Items API
  slug: doordash-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-items-api-openapi.yml
- filename: doordash-menus-api-openapi.yml
  format: yaml
  label: doordash Menus API
  slug: doordash-menus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-menus-api-openapi.yml
- filename: doordash-orders-api-openapi.yml
  format: yaml
  label: doordash Orders API
  slug: doordash-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-orders-api-openapi.yml
- filename: doordash-promotions-api-openapi.yml
  format: yaml
  label: doordash Promotions API
  slug: doordash-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-promotions-api-openapi.yml
- filename: doordash-quotes-api-openapi.yml
  format: yaml
  label: doordash Quotes API
  slug: doordash-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-quotes-api-openapi.yml
- filename: doordash-reports-api-openapi.yml
  format: yaml
  label: doordash Reports API
  slug: doordash-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-reports-api-openapi.yml
- filename: doordash-stores-api-openapi.yml
  format: yaml
  label: doordash Stores API
  slug: doordash-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/doordash-stores-api-openapi.yml
- filename: doordash-ads-openapi.yml
  format: yaml
  label: DoorDash Ads API
  slug: doordash-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/_original/doordash-ads-openapi.yml
- filename: doordash-storefront-openapi.yml
  format: yaml
  label: DoorDash Storefront API
  slug: doordash-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/_original/doordash-storefront-openapi.yml
- filename: doordash-parcel-openapi.yml
  format: yaml
  label: DoorDash Parcel API
  slug: doordash-parcel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/_original/doordash-parcel-openapi.yml
- filename: doordash-drive-refunds-openapi.yml
  format: yaml
  label: DoorDash Drive Refunds API
  slug: doordash-drive-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/_original/doordash-drive-refunds-openapi.yml
- filename: doordash-drive-redelivery-openapi.yml
  format: yaml
  label: DoorDash Drive Redelivery API
  slug: doordash-drive-redelivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/_original/doordash-drive-redelivery-openapi.yml
- filename: doordash-drive-dasher-feedback-openapi.yml
  format: yaml
  label: DoorDash Drive Dasher Feedback API
  slug: doordash-drive-dasher-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/_original/doordash-drive-dasher-feedback-openapi.yml
- filename: doordash-external-checkout-openapi.yml
  format: yaml
  label: DoorDash Checkout API
  slug: doordash-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/_original/doordash-external-checkout-openapi.yml
- filename: doordash-marketplace-legacy-openapi.yml
  format: yaml
  label: DoorDash Marketplace (legacy) API
  slug: doordash-marketplace-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/openapi/_original/doordash-marketplace-legacy-openapi.yml
auth_types:
- http
- apiKey
description: 'Every DoorDash developer API authenticates with a self-signed JSON Web Token presented as a bearer token. There is no OAuth flow, no token endpoint and no refresh: the caller mints a short-lived HS256 JWT locally from three credentials issued in the Developer Portal (developer_id, key_id, signing_secret) and signs it with the base64-decoded secret. Sandbox and production are separated by which access key is used, not by hostname. The Ads API and the legacy Marketplace API are the exceptions - both declare a plain apiKey-in-Authorization scheme in their own OpenAPI rather than the DoorDash JWT.'
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Doordash Authentication
name_suffix: Authentication
oauth_flows: []
overview: Doordash secures its APIs with http and apiKey across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Doordash
provider_slug: doordash
scheme_count: 5
schemes:
- agent_note: Because the token is minted locally and expires in at most 30 minutes, an agent must re-sign per session rather than cache a long-lived credential, and a 401 is almost always an expired token rather than a revoked key.
  applies_to:
  - Drive API
  - Drive (classic) API
  - Marketplace API
  - Item Management API
  - Reporting API
  - Parcel API
  - Drive Refunds API
  - Drive Redelivery API
  - Drive Dasher Feedback API
  - Storefront API
  bearerFormat: JWT
  credential_source: Developer Portal > Credentials. An access key is a triple of developer_id, key_id and signing_secret. Keys are scoped to an environment (Sandbox or Production).
  docs: https://developer.doordash.com/en-US/docs/drive/reference/JWTs
  header: 'Authorization: Bearer [JWT]'
  name: DoorDash JWT (bearer)
  scheme: bearer
  token:
    algorithm: HS256
    header_claims:
      alg: HS256
      dd-ver: DD-JWT-V1
      typ: JWT
    max_lifetime_seconds: 1800
    payload_claims:
    - description: Audience. Always the literal string "doordash".
      name: aud
      value: doordash
    - description: Issuer. The Developer ID (UUID).
      name: iss
    - description: Key ID (UUID) of the key used to sign the JWT.
      name: kid
    - description: Issued At, seconds from the epoch. Cannot be in the future.
      name: iat
    - description: Expiration, seconds from the epoch. Maximum 30 minutes (1800 seconds) beyond iat. The get-started tutorial signs tokens with exp = iat + 300.
      name: exp
    self_signed: true
    signing_key: the signing_secret, base64-decoded before use
  type: http
- applies_to:
  - DoorDash Ads API
  header_name: Authorization
  in: header
  name: Ads API Key Authentication
  note: Declared in the Ads OpenAPI as apiKey-in-header with the value carried as a bearer token. The Ads API is a separate advertising product surface from the logistics APIs.
  scheme_hint: bearer
  source: openapi/_original/doordash-ads-openapi.yml
  type: apiKey
- applies_to:
  - DoorDash Checkout API Interface
  header_name: Authorization
  in: header
  name: Drive API Key Authentication
  source: openapi/_original/doordash-external-checkout-openapi.yml
  type: apiKey
- applies_to:
  - Marketplace (legacy) API
  header_name: Authorization
  in: header
  name: Authorization
  note: Served from pointofsale.doordash.com; the legacy POS integration surface.
  source: openapi/_original/doordash-marketplace-legacy-openapi.yml
  type: apiKey
- applies_to:
  - Storefront V1 API
  name: BearerAuth
  scheme: bearer
  source: openapi/_original/doordash-storefront-openapi.yml
  type: http
slug: doordash-authentication
source_filename: doordash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: https://developer.doordash.com/en-US/docs/drive/reference/JWTs, https://developer.doordash.com/en-US/docs/drive/tutorials/get_started/, openapi/_original/\nprovider: doordash\ndescription: >-\n  Every DoorDash developer API authenticates with a self-signed JSON Web Token presented as a\n  bearer token. There is no OAuth flow, no token endpoint and no refresh: the caller mints a\n  short-lived HS256 JWT locally from three credentials issued in the Developer Portal\n  (developer_id, key_id, signing_secret) and signs it with the base64-decoded secret. Sandbox and\n  production are separated by which access key is used, not by hostname. The Ads API and the legacy\n  Marketplace API are the exceptions - both declare a plain apiKey-in-Authorization scheme in their\n  own OpenAPI rather than the DoorDash JWT.\nsummary:\n  types:\n  - http\n  - apiKey\n  primary: self-signed HS256 JWT presented as an Authorization bearer token\n  oauth2:\
  \ false\n  openid_connect: false\n  mtls: false\n  scopes: false\n  note: >-\n    No OAuth 2.0 or OpenID Connect surface exists anywhere on the estate; the\n    /.well-known/oauth-authorization-server and /.well-known/openid-configuration probes returned\n    404 on openapi.doordash.com and on the docs host. OAuth appears only in the opposite direction -\n    DoorDash can authenticate ITSELF to a partner's webhook endpoint using Basic Auth or OAuth\n    credentials the partner configures in the Developer Portal.\nschemes:\n- name: DoorDash JWT (bearer)\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  header: 'Authorization: Bearer [JWT]'\n  applies_to:\n  - Drive API\n  - Drive (classic) API\n  - Marketplace API\n  - Item Management API\n  - Reporting API\n  - Parcel API\n  - Drive Refunds API\n  - Drive Redelivery API\n  - Drive Dasher Feedback API\n  - Storefront API\n  docs: https://developer.doordash.com/en-US/docs/drive/reference/JWTs\n  credential_source: >-\n    Developer\
  \ Portal > Credentials. An access key is a triple of developer_id, key_id and\n    signing_secret. Keys are scoped to an environment (Sandbox or Production).\n  token:\n    self_signed: true\n    algorithm: HS256\n    signing_key: the signing_secret, base64-decoded before use\n    header_claims:\n      alg: HS256\n      typ: JWT\n      dd-ver: DD-JWT-V1\n    payload_claims:\n    - name: aud\n      value: doordash\n      description: Audience. Always the literal string \"doordash\".\n    - name: iss\n      description: Issuer. The Developer ID (UUID).\n    - name: kid\n      description: Key ID (UUID) of the key used to sign the JWT.\n    - name: iat\n      description: Issued At, seconds from the epoch. Cannot be in the future.\n    - name: exp\n      description: >-\n        Expiration, seconds from the epoch. Maximum 30 minutes (1800 seconds) beyond iat. The\n        get-started tutorial signs tokens with exp = iat + 300.\n    max_lifetime_seconds: 1800\n  agent_note: >-\n    Because\
  \ the token is minted locally and expires in at most 30 minutes, an agent must re-sign\n    per session rather than cache a long-lived credential, and a 401 is almost always an expired\n    token rather than a revoked key.\n- name: Ads API Key Authentication\n  type: apiKey\n  in: header\n  header_name: Authorization\n  scheme_hint: bearer\n  applies_to:\n  - DoorDash Ads API\n  source: openapi/_original/doordash-ads-openapi.yml\n  note: >-\n    Declared in the Ads OpenAPI as apiKey-in-header with the value carried as a bearer token. The\n    Ads API is a separate advertising product surface from the logistics APIs.\n- name: Drive API Key Authentication\n  type: apiKey\n  in: header\n  header_name: Authorization\n  applies_to:\n  - DoorDash Checkout API Interface\n  source: openapi/_original/doordash-external-checkout-openapi.yml\n- name: Authorization\n  type: apiKey\n  in: header\n  header_name: Authorization\n  applies_to:\n  - Marketplace (legacy) API\n  source: openapi/_original/doordash-marketplace-legacy-openapi.yml\n\
  \  note: Served from pointofsale.doordash.com; the legacy POS integration surface.\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  applies_to:\n  - Storefront V1 API\n  source: openapi/_original/doordash-storefront-openapi.yml\nenvironments:\n- name: Sandbox\n  self_serve: true\n  separation: by access key, not by hostname\n  note: >-\n    Self-serve signup requires only name, phone number and email. Sandbox deliveries are simulated\n    and are never dispatched to a Dasher.\n- name: Production\n  self_serve: false\n  separation: by access key, not by hostname\n  note: >-\n    Production access to the Drive API is restricted and requires a certification review; DoorDash\n    states it cannot provide a timeline. Marketplace APIs are not generally available and require\n    an application from the Developer Portal Integrations tab.\nwebhook_authentication:\n  direction: DoorDash -> partner\n  docs: https://developer.doordash.com/en-US/docs/drive/how_to/webhooks\n  requirements:\n\
  \  - The receiving endpoint must be HTTPS.\n  - One endpoint per environment (Sandbox and Production each support exactly one).\n  methods:\n  - name: Basic Auth\n    description: The partner supplies the exact contents DoorDash should send in the Authorization header.\n  - name: OAuth\n    description: >-\n      The partner supplies a client ID, client secret, a token URL DoorDash requests a token from,\n      and an optional scope.\n  signature_verification: false\n  note: >-\n    DoorDash does NOT sign webhook payloads with a shared secret or an HMAC header. Authenticity is\n    established by the partner requiring credentials on its own endpoint, which means a partner who\n    leaves the endpoint open has no cryptographic way to verify a payload came from DoorDash.\ngaps:\n- >-\n  Nine of the thirteen published OpenAPI documents declare no securitySchemes at all - the JWT\n  requirement lives only in prose on the docs site, so a client generated from the Drive,\n  Marketplace, Item\
  \ Management, Reporting or Parcel spec alone would emit unauthenticated requests.\n- No published key-rotation policy, no token revocation endpoint, and no documented scope surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/authentication/doordash-authentication.yml
summary_line: http/apiKey · 5 schemes
tags:
- Delivery
- Logistics
- Last Mile Delivery
- On-Demand
- Food Delivery
- Local Commerce
- Marketplace
- Restaurant
- Grocery
- Retail
- Fulfillment
- Webhook
---
