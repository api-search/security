---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ccpa-drop-databroker-api.yml
  format: yaml
  label: CalPrivacy DROP Data Broker API
  slug: drop-data-broker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ccpa/refs/heads/main/openapi/ccpa-drop-databroker-api.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ccpa Authentication
name_suffix: Authentication
oauth_flows: []
overview: CCPA (California Consumer Privacy Act) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CCPA (California Consumer Privacy Act)
provider_slug: ccpa
scheme_count: 1
schemes:
- applied: global
  description: API key issued through the Data Broker Portal. The key grants access only to the consumer deletion lists selected during setup.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/ccpa-drop-databroker-api.yml
  - https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/getting-started/
  type: apiKey
slug: ccpa-authentication
source_filename: ccpa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/getting-started/\n  (docs) enriching openapi/ccpa-drop-databroker-api.yml (spec)\ndocs: https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/getting-started/\nprovider: CCPA (California Consumer Privacy Act)\nproviderId: ccpa\napi: ccpa:drop-data-broker-api\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: X-API-KEY\n    description: >-\n      API key issued through the Data Broker Portal. The key grants access only to the\n      consumer deletion lists selected during setup.\n    applied: global\n    sources:\n      - openapi/ccpa-drop-databroker-api.yml\n      - https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/getting-started/\nkey_lifecycle:\n\
  \  issuance: >-\n    Keys are generated in the DROP Data Broker Portal (https://databroker.drop.privacy.ca.gov/)\n    after data broker registration and fee payment are complete. Sign in, go to\n    Home > Consumer Deletion Lists, select the list type(s), Save, then open the API Key tab\n    and choose \"Get a new API key\".\n  sandbox_issuance: >-\n    A separate sandbox key is issued from SANDBOX ENVIRONMENT > ISSUE SANDBOX API KEY in the\n    same portal.\n  rotation: >-\n    Provider guidance: \"Store keys securely using environment variables or secret management\n    systems. Regenerate keys if compromised or if list selection changes.\" Issuing a new key\n    deactivates all previous keys (notification event \"API Key Changed\").\n  scoping: >-\n    A key is scoped to the consumer deletion list types selected during setup (NDZ, Email,\n    Phone, MAID, NameVIN, CTVID). Changing list selection requires regenerating the key.\n  authorization_model: >-\n    Per-data-broker credential\
  \ tied to a registered CalPrivacy data broker account. There is\n    no OAuth, no scopes surface, and no delegated/third-party authorization flow.\nfailure_modes:\n  - status: 401\n    body: 'API key is missing or invalid. Fix or regenerate the API key and try again.'\n    observed: >-\n      Live unauthenticated GET https://api.drop.privacy.ca.gov/data/download on 2026-09-05\n      returned 401 with this plain-text body (not application/problem+json).\n  - status: 403\n    meaning: Key is valid but the account is not authorized for the requested list or action.\nnotes: >-\n  This is a REGULATOR-operated API. The credential is issued as part of a statutory\n  registration process under the California Delete Act (Civil Code 1798.99.80 et seq.),\n  not through self-service signup, and carries an annual fee.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ccpa/refs/heads/main/authentication/ccpa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CPRA
- California
- Compliance
- Data Protection
- Data Subject Rights
- Legal
- Privacy
- Regulations
---
