---
api_key_in:
- header
api_specs:
- filename: n3rgy-customer-service-api-v2-openapi.yaml
  format: yaml
  label: n3rgy Customer Service API V2
  slug: customer-service-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/openapi/n3rgy-customer-service-api-v2-openapi.yaml
auth_types:
- apiKey
description: n3rgy authenticates with a single API key in the x-api-key header — and then authorises in two further layers that the OpenAPI cannot express. Layer 2 is end-customer CONSENT, validated server-side against the Home Area Network behind the supplied MPxN. Layer 3 is a per-account permission to change meter update frequencies. All three failures surface as HTTP 403 with different messages, so a client cannot distinguish "bad key" from "no consent" by status code alone — only by the message string.
kind: authentication
layout: security
method: searched
name: N3Rgy Authentication
name_suffix: Authentication
oauth_flows: []
overview: n3rgy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: n3rgy
provider_slug: n3rgy
scheme_count: 1
schemes:
- applies_to: 25 of 26 operations
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/n3rgy-customer-service-api-v2-openapi.yaml
  type: apiKey
  x-amazon-apigateway-api-key-source: HEADER
slug: n3rgy-authentication
source_filename: n3rgy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/n3rgy-customer-service-api-v2-openapi.yaml\ndocs: https://customer-api-user-manuals.data.n3rgy.com/authentication/\ndocs_sandbox: https://customer-api-user-manuals.data.n3rgy.com/sandbox-authentication/\ndescription: >-\n  n3rgy authenticates with a single API key in the x-api-key header — and then\n  authorises in two further layers that the OpenAPI cannot express. Layer 2 is\n  end-customer CONSENT, validated server-side against the Home Area Network\n  behind the supplied MPxN. Layer 3 is a per-account permission to change meter\n  update frequencies. All three failures surface as HTTP 403 with different\n  messages, so a client cannot distinguish \"bad key\" from \"no consent\" by status\n  code alone — only by the message string.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oidc: false\n  mtls: false\n  authorization_layers: 3\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n\
  \  in: header\n  parameter: x-api-key\n  x-amazon-apigateway-api-key-source: HEADER\n  sources:\n  - openapi/n3rgy-customer-service-api-v2-openapi.yaml\n  applies_to: 25 of 26 operations\n\nkey_provisioning:\n  self_serve: false\n  live: >-\n    \"Access to the Customer Service API must be enabled for the user's live API\n    key by the n3rgy data backoffice.\"\n  sandbox: >-\n    \"Access to the Customer Service API Sandbox must be enabled for the user's\n    sandbox API key by the n3rgy data backoffice.\"\n  steps:\n    - Read the developer guide anonymously — no login required.\n    - Complete the business sign-up form at https://data.n3rgy.com/business-sign-up (free sandbox tier).\n    - Contact n3rgy to have the live key enabled by the back office.\n    - Obtain end-customer consent per property before any consent-bearing endpoint returns data.\n  environment_separation: by hostname, not by key prefix (see sandbox/n3rgy-sandbox.yml)\n  key_prefixes: none published\n  rotation_policy:\
  \ not published\n\nauthorization_layers:\n  - layer: 1\n    name: API key\n    mechanism: x-api-key header\n    failure: 403 \"User is not authorized to access this resource with an explicit deny.\"\n    applies_to: all operations except RetrieveReadingTypeData\n  - layer: 2\n    name: consent verification\n    mechanism: >-\n      Server-side check that an ACTIVE consent exists for the HAN identified by\n      the supplied MPxN. Consent is granted and withdrawn by the occupant through\n      the n3rgy Consumer Portal (https://data.n3rgy.com/consumer-login), not\n      through this API.\n    failures:\n      - 403 \"Consent for the given MPxN not found.\"\n      - 403 \"Consent for the given MPxN does not have update frequencies set.\"\n      - 403 \"Consent for the property of the target meter not found.\"\n    applies_to:\n      - RetrieveConsentedMPxNUtilities\n      - RetrieveDataTypesForUtility\n      - RetrieveDataUpdateFrequencies\n      - RetrieveDataForReadingType\n      - generateFetchNowRequest\n\
  \      - SetMeterUpdateFrequency\n  - layer: 3\n    name: frequency-change permission\n    mechanism: A per-customer flag allowing update-frequency changes.\n    failure: 403 \"User is not authorized to access this resource with an explicit deny.\"\n    applies_to:\n      - SetMeterUpdateFrequency\n      - SetDefaults\n      - ResetAllUpdateFrequencies\n\nkey_only_operations:\n  note: Authenticated by x-api-key alone, with no consent check.\n  operations:\n    - RetrieveConsentedMPxNs\n    - RetrieveMPxNAvailability\n    - mpxnFromAddress\n    - ReadInventory\n    - GetPushNotificationConfiguration\n    - EditPushNotificationConfiguration\n    - DeletePushNotificationConfiguration\n    - RetrievePushNotificationStatus\n\nunsecured_operations:\n  - operationId: RetrieveReadingTypeData\n    path: POST /internal/{mpxn}/{utility}/{readingType}\n    note: >-\n      Declares an EMPTY security array in the OpenAPI (no ApiKeyAuth). Almost\n      certainly an internal endpoint fronted by other\
  \ controls — flagged here as a\n      contract inconsistency worth raising with the provider, not as a claim that\n      the endpoint is publicly callable. The host answers 403 to anonymous\n      callers.\n\nnot_supported:\n  oauth2: >-\n    No oauth2 securityScheme; no /.well-known/oauth-authorization-server on any\n    host. Therefore no scopes/ artifact is emitted — there is no scope surface.\n  openid_connect: >-\n    No /.well-known/openid-configuration is served anywhere (401 on\n    consumer-api.data.n3rgy.com, SPA HTML shell on data.n3rgy.com).\n  mutual_tls: not declared\n  http_basic_bearer: not declared\n\nhistory:\n  - >-\n    n3rgy data 1.x authenticated with the Authorization header. n3rgy data 2.0\n    migrated every endpoint to X-API-KEY (\"With n3rgy data 2.0, all new endpoints\n    will be using X-API-KEY as header parameter instead of the old authorization\n    header.\" — developer guide Overview).\n  - >-\n    The legacy consumer API authenticated with the IHD MAC\
  \ address of the\n    property's in-home display. That API has been withdrawn.\n\ncross_references:\n  conventions: conventions/n3rgy-conventions.yml\n  errors: errors/n3rgy-problem-types.yml\n  sandbox: sandbox/n3rgy-sandbox.yml\n  well_known: well-known/n3rgy-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/authentication/n3rgy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Energy
- United Kingdom
- Utilities
- Smart Metering
- Electricity
- Gas
- Smart Meter Data
- Consent
- Metering
- Energy Data
---
