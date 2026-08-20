---
api_key_in:
- header
api_specs:
- filename: bmo-account-validation-openapi.json
  format: json
  label: BMO Account Validation API
  slug: bmo-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-account-validation-openapi.json
- filename: bmo-account-information-openapi.json
  format: json
  label: BMO Account Information API
  slug: bmo-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-account-information-openapi.json
- filename: bmo-ach-payments-openapi.json
  format: json
  label: BMO ACH Payments API
  slug: bmo-ach-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-ach-payments-openapi.json
- filename: bmo-wire-payments-us-openapi.json
  format: json
  label: BMO Wire Payments (U.S.) API
  slug: bmo-wire-payments-us-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-wire-payments-us-openapi.json
- filename: bmo-wire-payments-ca-openapi.json
  format: json
  label: BMO Wire Payments (Canada) API
  slug: bmo-wire-payments-ca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-wire-payments-ca-openapi.json
- filename: bmo-eft-payments-openapi.json
  format: json
  label: BMO EFT Payments API
  slug: bmo-eft-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-eft-payments-openapi.json
- filename: bmo-interac-instant-payments-openapi.json
  format: json
  label: BMO Instant Payments (Interac) API
  slug: bmo-interac-instant-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-interac-instant-payments-openapi.json
- filename: bmo-image-retrieval-swagger.json
  format: json
  label: BMO Image Retrieval API
  slug: bmo-image-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-image-retrieval-swagger.json
- filename: bmo-authorize-token-swagger.json
  format: json
  label: BMO Authorize & Token API
  slug: bmo-authorize-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-authorize-token-swagger.json
- filename: bmo-client-data-encryption-key-swagger.json
  format: json
  label: BMO Client Data Encryption Key API
  slug: bmo-client-data-encryption-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-client-data-encryption-key-swagger.json
- filename: bmo-push-notification-openapi.json
  format: json
  label: BMO Push Notification API
  slug: bmo-push-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/openapi/bmo-push-notification-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bmo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BMO secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BMO
provider_slug: bmo
scheme_count: 3
schemes:
- in: header
  name: api-key-1
  parameter: x-api-key
  sources:
  - openapi/bmo-account-information-openapi.json
  - openapi/bmo-account-validation-openapi.json
  - openapi/bmo-ach-payments-openapi.json
  - openapi/bmo-client-data-encryption-key-swagger.json
  - openapi/bmo-eft-payments-openapi.json
  - openapi/bmo-image-retrieval-swagger.json
  - openapi/bmo-interac-instant-payments-openapi.json
  - openapi/bmo-push-notification-openapi.json
  - openapi/bmo-wire-payments-ca-openapi.json
  - openapi/bmo-wire-payments-us-openapi.json
  type: apiKey
- flows:
  - authorizationUrl: https://open-api.bmofg.com/open-banking/commercial-sb/oauth20/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://open-api.bmofg.com/open-banking/commercial-sb/oauth20/token
  name: OAuth
  sources:
  - openapi/bmo-account-information-openapi.json
  - openapi/bmo-account-validation-openapi.json
  - openapi/bmo-ach-payments-openapi.json
  - openapi/bmo-eft-payments-openapi.json
  - openapi/bmo-image-retrieval-swagger.json
  - openapi/bmo-interac-instant-payments-openapi.json
  - openapi/bmo-wire-payments-ca-openapi.json
  - openapi/bmo-wire-payments-us-openapi.json
  type: oauth2
- in: header
  name: clientIdHeader
  parameter: X-IBM-Client-Id
  sources:
  - openapi/bmo-authorize-token-swagger.json
  type: apiKey
slug: bmo-authentication
source_filename: bmo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/bmo-account-information-openapi.json, openapi/bmo-account-validation-openapi.json,\n  openapi/bmo-ach-payments-openapi.json, openapi/bmo-authorize-token-swagger.json, openapi/bmo-client-data-encryption-key-swagger.json,\n  openapi/bmo-eft-payments-openapi.json, openapi/bmo-image-retrieval-swagger.json, openapi/bmo-interac-instant-payments-openapi.json,\n  openapi/bmo-push-notification-openapi.json, openapi/bmo-wire-payments-ca-openapi.json, openapi/bmo-wire-payments-us-openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: api-key-1\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/bmo-account-information-openapi.json\n  - openapi/bmo-account-validation-openapi.json\n  - openapi/bmo-ach-payments-openapi.json\n  - openapi/bmo-client-data-encryption-key-swagger.json\n  - openapi/bmo-eft-payments-openapi.json\n\
  \  - openapi/bmo-image-retrieval-swagger.json\n  - openapi/bmo-interac-instant-payments-openapi.json\n  - openapi/bmo-push-notification-openapi.json\n  - openapi/bmo-wire-payments-ca-openapi.json\n  - openapi/bmo-wire-payments-us-openapi.json\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://open-api.bmofg.com/open-banking/commercial-sb/oauth20/authorize\n    tokenUrl: https://open-api.bmofg.com/open-banking/commercial-sb/oauth20/token\n    scopes: 1\n  sources:\n  - openapi/bmo-account-information-openapi.json\n  - openapi/bmo-account-validation-openapi.json\n  - openapi/bmo-ach-payments-openapi.json\n  - openapi/bmo-eft-payments-openapi.json\n  - openapi/bmo-image-retrieval-swagger.json\n  - openapi/bmo-interac-instant-payments-openapi.json\n  - openapi/bmo-wire-payments-ca-openapi.json\n  - openapi/bmo-wire-payments-us-openapi.json\n- name: clientIdHeader\n  type: apiKey\n  in: header\n  parameter: X-IBM-Client-Id\n  sources:\n  - openapi/bmo-authorize-token-swagger.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bmo/refs/heads/main/authentication/bmo-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Financial-Services
- Banking
- United States
- Open Finance
- Payments
- Commercial Banking
- Treasury Management
- Account Validation
---
