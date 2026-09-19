---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: agl-agltosupplier-api-openapi.yml
  format: yaml
  label: AGL AGL To Supplier API
  slug: agl-agltosupplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-agltosupplier-api-openapi.yml
- filename: agl-codes-api-openapi.yml
  format: yaml
  label: AGL Codes API
  slug: agl-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-codes-api-openapi.yml
- filename: agl-golf-clubs-api-openapi.yml
  format: yaml
  label: AGL Golf Clubs API
  slug: agl-golf-clubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-golf-clubs-api-openapi.yml
- filename: agl-reservation-api-openapi.yml
  format: yaml
  label: AGL Reservation API
  slug: agl-reservation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-reservation-api-openapi.yml
- filename: agl-reservations-api-openapi.yml
  format: yaml
  label: AGL Reservations API
  slug: agl-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-reservations-api-openapi.yml
- filename: agl-static-packages-api-openapi.yml
  format: yaml
  label: AGL Static Packages API
  slug: agl-static-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-static-packages-api-openapi.yml
- filename: agl-suppliertoagl-api-openapi.yml
  format: yaml
  label: AGL Supplier To AGL API
  slug: agl-suppliertoagl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-suppliertoagl-api-openapi.yml
- filename: agl-tee-times-api-openapi.yml
  format: yaml
  label: AGL Tee Times API
  slug: agl-tee-times-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-tee-times-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 8
method: searched
name: Agl Authentication
name_suffix: Authentication
oauth_flows: []
overview: AGL secures its APIs with apiKey and http across 9 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AGL
provider_slug: agl
scheme_count: 9
schemes:
- api: AGL OPEN API
  applied: globally via the root security block
  bearerFormat: SHA-256
  docs_note: '"All APIs are secured using SHA-256-based Authorization and require proper identification headers." - AGL OPEN API info.description.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/agl-open-openapi-original.yml
  type: http
- api: AGL OPEN API
  description: Supplier code issued by AGL. Required on every SupplierToAGL operation.
  in: header
  name: X-Supplier-Code
  parameter: X-Supplier-Code
  required: true
  sources:
  - openapi/agl-open-openapi-original.yml
  type: identification-header
- api: AGL OPEN API
  description: Client code issued by the supplier to AGL. Required on the AGLToSupplier operations - the callbacks AGL makes into the supplier's endpoint.
  in: header
  name: X-Client-Code
  parameter: X-Client-Code
  required: true
  sources:
  - openapi/agl-open-openapi-original.yml
  type: identification-header
- api: AGL OTA API
  applied: globally via the root security block
  in: header
  name: bearerAuth
  note: Declared as an apiKey in the Authorization header rather than as http/bearer, so the contract does not state whether the value is prefixed "Bearer ".
  parameter: Authorization
  sources:
  - openapi/agl-ota-openapi-original.yml
  type: apiKey
- api: AGL OTA API
  applied: globally via the root security block
  description: Partner identifier issued by AGL, sent alongside the Authorization token.
  in: header
  name: clientId
  parameter: clientId
  sources:
  - openapi/agl-ota-openapi-original.yml
  type: apiKey
- api: AGL Trip.com Reservation Integration API
  bearerFormat: JWT
  name: Bearer
  scheme: Bearer
  sources:
  - openapi/agl-tripcom-outbound-openapi-original.yml
  type: http
- api: AGL Trip.com Reservation Integration API
  in: header
  name: ClientId
  parameter: ClientId
  sources:
  - openapi/agl-tripcom-outbound-openapi-original.yml
  type: apiKey
- api: AGL Trip.com Reservation Integration API
  in: header
  name: Currency
  note: Declared as a securityScheme but is a content-negotiation header, not a credential. Recorded as the contract declares it.
  parameter: Currency
  sources:
  - openapi/agl-tripcom-outbound-openapi-original.yml
  type: apiKey
- api: AGL Trip.com Reservation Integration API
  in: header
  name: Language
  note: Same as Currency - declared as a securityScheme but is not a credential.
  parameter: Language
  sources:
  - openapi/agl-tripcom-outbound-openapi-original.yml
  type: apiKey
slug: agl-authentication
source_filename: agl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: >-\n  openapi/agl-open-openapi-original.yml, openapi/agl-ota-openapi-original.yml,\n  openapi/agl-tripcom-outbound-openapi-original.yml\ndocs: >-\n  https://api-docs-agl-bridgeapi.tigergds.com/reference (AGL OPEN API info.description states the\n  header contract in prose), https://api-doc.tigergds.com/reference\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  oidc: false\n  mutual_tls: false\n  credential_issuance: >-\n    Manual. Credentials are issued per partner after the partnership application at\n    https://www.aglgw.com/en/partners or the TIGER GDS partner sign-up at\n    https://www.tigergds.com/signup/step1. There is no self-service key creation, no key-rotation\n    operation and no scope model anywhere in the platform.\n  request_signing: >-\n    Two of the three surfaces sign requests. The AGL OPEN API's Authorization header carries a\n    \"Bearer <SHA-256 hashed\
  \ signature>\", and the Trip.com outbound bridge carries a sign value\n    alongside accountId, serviceName, requestTime and version in its request-header object.\n    Neither publishes the canonical string-to-sign, so neither signature can be implemented from\n    the public documentation alone - it has to come from AGL during onboarding.\nschemes:\n- name: bearerAuth\n  api: AGL OPEN API\n  type: http\n  scheme: bearer\n  bearerFormat: SHA-256\n  applied: globally via the root security block\n  docs_note: >-\n    \"All APIs are secured using SHA-256-based Authorization and require proper identification\n    headers.\" - AGL OPEN API info.description.\n  sources: [openapi/agl-open-openapi-original.yml]\n- name: X-Supplier-Code\n  api: AGL OPEN API\n  type: identification-header\n  in: header\n  parameter: X-Supplier-Code\n  required: true\n  description: Supplier code issued by AGL. Required on every SupplierToAGL operation.\n  sources: [openapi/agl-open-openapi-original.yml]\n- name:\
  \ X-Client-Code\n  api: AGL OPEN API\n  type: identification-header\n  in: header\n  parameter: X-Client-Code\n  required: true\n  description: >-\n    Client code issued by the supplier to AGL. Required on the AGLToSupplier operations - the\n    callbacks AGL makes into the supplier's endpoint.\n  sources: [openapi/agl-open-openapi-original.yml]\n- name: bearerAuth\n  api: AGL OTA API\n  type: apiKey\n  in: header\n  parameter: Authorization\n  applied: globally via the root security block\n  note: >-\n    Declared as an apiKey in the Authorization header rather than as http/bearer, so the contract\n    does not state whether the value is prefixed \"Bearer \".\n  sources: [openapi/agl-ota-openapi-original.yml]\n- name: clientId\n  api: AGL OTA API\n  type: apiKey\n  in: header\n  parameter: clientId\n  applied: globally via the root security block\n  description: Partner identifier issued by AGL, sent alongside the Authorization token.\n  sources: [openapi/agl-ota-openapi-original.yml]\n\
  - name: Bearer\n  api: AGL Trip.com Reservation Integration API\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  sources: [openapi/agl-tripcom-outbound-openapi-original.yml]\n- name: ClientId\n  api: AGL Trip.com Reservation Integration API\n  type: apiKey\n  in: header\n  parameter: ClientId\n  sources: [openapi/agl-tripcom-outbound-openapi-original.yml]\n- name: Currency\n  api: AGL Trip.com Reservation Integration API\n  type: apiKey\n  in: header\n  parameter: Currency\n  note: >-\n    Declared as a securityScheme but is a content-negotiation header, not a credential. Recorded\n    as the contract declares it.\n  sources: [openapi/agl-tripcom-outbound-openapi-original.yml]\n- name: Language\n  api: AGL Trip.com Reservation Integration API\n  type: apiKey\n  in: header\n  parameter: Language\n  note: Same as Currency - declared as a securityScheme but is not a credential.\n  sources: [openapi/agl-tripcom-outbound-openapi-original.yml]\nscopes:\n  supported: false\n  note: >-\n\
  \    No OAuth 2.0 and therefore no scope surface. Authorization is all-or-nothing per issued\n    credential, differentiated only by partner type (Provider Partner or Seller Partner, chosen at\n    sign-up) and by which of the two contracts the partner is given access to. No scopes/ artifact\n    is written - there is nothing to enumerate.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/authentication/agl-authentication.yml
summary_line: apiKey/http · 9 schemes
tags:
- Company
- Golf
- Travel
- Booking
- Reservations
- Distribution
- Tee Times
- GDS
- Hospitality
- Sports
- Leisure
- South Korea
---
