---
api_key_in: []
api_specs:
- filename: treez-dispensary-openapi.json
  format: json
  label: Treez Dispensary API v3
  slug: treez-dispensary-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/openapi/treez-dispensary-openapi.json
- filename: treez-catalog-openapi.json
  format: json
  label: Treez Catalog Service API
  slug: treez-catalog-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/openapi/treez-catalog-openapi.json
- filename: treez-discount-openapi.json
  format: json
  label: Treez Discount Service API
  slug: treez-discount-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/openapi/treez-discount-openapi.json
- filename: treez-collections-openapi.json
  format: json
  label: Treez Collection Service API
  slug: treez-collection-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/openapi/treez-collections-openapi.json
- filename: treez-tag-openapi.json
  format: json
  label: Treez Tag Service API
  slug: treez-tag-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/openapi/treez-tag-openapi.json
- filename: treez-jwt-check-openapi.json
  format: json
  label: Treez JWT Validation Service
  slug: treez-jwt-validation-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/openapi/treez-jwt-check-openapi.json
- filename: treez-product-api-openapi.json
  format: json
  label: Treez Legacy SellTreez v2.0 Product API
  slug: treez-legacy-selltreez-v20-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/openapi/treez-product-api-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Treez Authentication
name_suffix: Authentication
oauth_flows: []
overview: Treez declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Treez
provider_slug: treez
scheme_count: 2
schemes:
- applies_to:
  - openapi/treez-dispensary-openapi.json
  - openapi/treez-catalog-openapi.json
  - openapi/treez-discount-openapi.json
  - openapi/treez-tag-openapi.json
  - openapi/treez-collections-openapi.json
  - openapi/treez-jwt-check-openapi.json
  claims:
    aud: The exact API endpoint URL being called
    exp: Expiry, in milliseconds - must be iat + 30000
    iat: Issued-at, in MILLISECONDS since epoch
    iss: Certificate ID (the integrator identifier Treez issues against the stored public key)
    jti: Recommended unique token id to prevent replay
    oid: Organization ID (GUID of the organization the call is destined for)
  description: Every request to the v3 Dispensary and Service APIs carries a self-signed JWT in the Authorization header. The integrator generates an RSA-4096 key pair, sends the public key (.crt) to api-support@treez.io, and Treez returns a Certificate ID bound to a record listing the organizations, dispensaries and endpoints that integrator is entitled to call. Requests are signed with the corresponding private key using RSA-SHA256; the token value is base64url(header) + "." + base64(signature).
  header_format: 'Authorization: <base64url-encoded-claims>.<base64-RSA-SHA256-signature>'
  id: self-signed-jwt
  in: header
  key_management:
    algorithm: RSA
    generation: openssl req -new -newkey rsa:4096 -x509 -sha256 -days 1825 -noenc -out public.crt -keyout private.key
    key_size: 4096
    public_key_delivery: email the .crt to api-support@treez.io
    rotation: Access to additional organizations, dispensaries and endpoints is added or revoked by updating the certificate record Treez holds against the public key. The docs do not state a rotation cadence or a self-service key-rotation endpoint.
    signature: SHA256withRSA
  name: Authorization
  scheme: bearer-like
  scoping: One certificate can be granted access to many organizations and dispensaries; the docs call this a "flexible one-to-many design" that removes the need for a per-dispensary API key.
  standard: RFC 7519 (JSON Web Token)
  ttl:
    enforced: true
    note: Treez enforces a 30,000 ms TTL; a TTL outside that range returns a 400.
    on_violation: HTTP 400
    value_ms: 30000
  type: http
  validation_endpoint:
    description: Check the validity of a signed JWT and view the resources it has been granted access to.
    method: POST
    operationId: post_jwt-validation
    spec: openapi/treez-jwt-check-openapi.json
    url: https://api-prod.treez.io/service/jwt-validation
- applies_to:
  - openapi/treez-product-api-openapi.json
  credential_issuance: Mutual customers request a production API key on the partner's behalf via Treez support (https://support.treez.io/).
  description: The legacy SellTreez v2 surface (api.treez.io/v2.0/dispensary, the Product API) uses an Authorization API that exchanges a partner client ID plus a per-location API key for an access token. Client IDs are issued once per partner at onboarding and never change; a separate API key is generated for each Treez retail location the partner integrates with, and production keys are only issued after the partner completes certification.
  id: legacy-client-id-api-key
  in: header
  status: legacy
  token:
    lifetime: 2 hours
    note: Treez requires certified partners to call the Authorization API only when the current token expires or shortly before; inefficient re-authentication is grounds for refusing certification.
  type: apiKey
slug: treez-authentication
source_filename: treez-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\ndocs: https://code.treez.io/reference/authentication\nsource: >-\n  https://code.treez.io/reference/authentication (self-signed JWT scheme, current v3 APIs) and\n  https://code.treez.io/docs/authorization-2 (legacy client-ID/API-key Authorization API for the\n  SellTreez v2 surface). Neither is expressible from the OpenAPI documents: all seven published\n  definitions declare an EMPTY components.securitySchemes and no security[] requirement, so a\n  derive-only pass (0-working/derive-authentication.py) returns nothing. This file is the\n  documented reality the specs omit.\nsummary:\n  auth_types: [jwt-self-signed, api-key]\n  primary: jwt-self-signed\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  api_key_locations: [header]\n  spec_declared: false\n  spec_gap: >-\n    All 7 OpenAPI definitions omit securitySchemes entirely. An agent reading only the contract\n    cannot tell how to authenticate; it must read the\
  \ prose auth page.\nschemes:\n- id: self-signed-jwt\n  type: http\n  scheme: bearer-like\n  in: header\n  name: Authorization\n  applies_to:\n  - openapi/treez-dispensary-openapi.json\n  - openapi/treez-catalog-openapi.json\n  - openapi/treez-discount-openapi.json\n  - openapi/treez-tag-openapi.json\n  - openapi/treez-collections-openapi.json\n  - openapi/treez-jwt-check-openapi.json\n  standard: RFC 7519 (JSON Web Token)\n  description: >-\n    Every request to the v3 Dispensary and Service APIs carries a self-signed JWT in the\n    Authorization header. The integrator generates an RSA-4096 key pair, sends the public key\n    (.crt) to api-support@treez.io, and Treez returns a Certificate ID bound to a record listing\n    the organizations, dispensaries and endpoints that integrator is entitled to call. Requests\n    are signed with the corresponding private key using RSA-SHA256; the token value is\n    base64url(header) + \".\" + base64(signature).\n  header_format: 'Authorization: <base64url-encoded-claims>.<base64-RSA-SHA256-signature>'\n\
  \  claims:\n    aud: The exact API endpoint URL being called\n    iss: Certificate ID (the integrator identifier Treez issues against the stored public key)\n    oid: Organization ID (GUID of the organization the call is destined for)\n    iat: Issued-at, in MILLISECONDS since epoch\n    exp: Expiry, in milliseconds - must be iat + 30000\n    jti: Recommended unique token id to prevent replay\n  ttl:\n    value_ms: 30000\n    enforced: true\n    on_violation: HTTP 400\n    note: Treez enforces a 30,000 ms TTL; a TTL outside that range returns a 400.\n  key_management:\n    algorithm: RSA\n    key_size: 4096\n    signature: SHA256withRSA\n    generation: 'openssl req -new -newkey rsa:4096 -x509 -sha256 -days 1825 -noenc -out public.crt -keyout private.key'\n    public_key_delivery: email the .crt to api-support@treez.io\n    rotation: >-\n      Access to additional organizations, dispensaries and endpoints is added or revoked by\n      updating the certificate record Treez holds against\
  \ the public key. The docs do not state\n      a rotation cadence or a self-service key-rotation endpoint.\n  scoping: >-\n    One certificate can be granted access to many organizations and dispensaries; the docs call\n    this a \"flexible one-to-many design\" that removes the need for a per-dispensary API key.\n  validation_endpoint:\n    operationId: post_jwt-validation\n    method: POST\n    url: https://api-prod.treez.io/service/jwt-validation\n    spec: openapi/treez-jwt-check-openapi.json\n    description: Check the validity of a signed JWT and view the resources it has been granted access to.\n- id: legacy-client-id-api-key\n  type: apiKey\n  in: header\n  status: legacy\n  applies_to:\n  - openapi/treez-product-api-openapi.json\n  description: >-\n    The legacy SellTreez v2 surface (api.treez.io/v2.0/dispensary, the Product API) uses an\n    Authorization API that exchanges a partner client ID plus a per-location API key for an access\n    token. Client IDs are issued once per\
  \ partner at onboarding and never change; a separate API\n    key is generated for each Treez retail location the partner integrates with, and production\n    keys are only issued after the partner completes certification.\n  token:\n    lifetime: 2 hours\n    note: >-\n      Treez requires certified partners to call the Authorization API only when the current token\n      expires or shortly before; inefficient re-authentication is grounds for refusing\n      certification.\n  credential_issuance: >-\n    Mutual customers request a production API key on the partner's behalf via Treez support\n    (https://support.treez.io/).\nonboarding:\n  self_serve: false\n  gate: partner application + MNDA + API Usage Agreement + certification\n  application_url: https://www.treez.io/partner-application\n  process_url: https://code.treez.io/page/partner-with-us\n  agreement_url: https://code.treez.io/page/legal\n  sandbox_before_production: true\n  contacts:\n    partnerships: partners@treez.io\n \
  \   technical: api-support@treez.io\n    support: support@treez.io\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/authentication/treez-authentication.yml
summary_line: 2 schemes
tags:
- cannabis
- point-of-sale
- Retail
- dispensary
- inventory-management
- E-Commerce
- Payments
- Compliance
- Track and Trace
- metrc
- product-catalog
- customer-data
---
