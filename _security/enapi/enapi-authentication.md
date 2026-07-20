---
api_key_in: []
auth_types:
- ocpi-token
description: ''
kind: authentication
layout: security
method: searched
name: Enapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enapi secures its APIs with ocpi-token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Enapi
provider_slug: enapi
scheme_count: 1
schemes:
- encoding:
    base64_header_2_2_1_plus: OCPI 2.2.1+ introduced Base64 encoding of the token in the Authorization header. The token value in the credentials body is unchanged; only the header representation differs. Configured per connection to match the partner platform.
  handshake:
    enapi_party_id: DE*ENA
    methods:
    - enapi-initiates: partner provides Versions URL + Token A; Enapi initiates
    - partner-initiates: Enapi provides its Versions URL + Token A; partner initiates
    module: Credentials
    setup: Portal > Settings > Roaming Settings > New Handshake (4-step wizard)
    versions_url_production: https://roaming.enapi.com/ocpi/versions
    versions_url_staging: https://roaming.staging.enapi.com/ocpi/versions
  header: Authorization
  in: header
  name: OCPI Token
  sources:
  - docs://getting-started/set-up-your-ocpi-handshake-with-enapi
  - docs://technical-documentation/supported-ocpi-modules-and-capabilities
  type: token
slug: enapi-authentication
source_filename: enapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.enapi.com/getting-started/set-up-your-ocpi-handshake-with-enapi\ndocs: https://docs.enapi.com/getting-started/set-up-your-ocpi-handshake-with-enapi\nsummary:\n  types: [ocpi-token]\n  model: OCPI credentials handshake (token exchange)\n  transport: Authorization header\n  note: >-\n    Enapi does not expose a proprietary auth scheme. Access follows the OCPI\n    Credentials module: a one-time handshake exchanges credentials between partner\n    and Enapi, producing a credential (token) pair. There is no OAuth2/OpenID\n    Connect and no OAuth scope surface.\nschemes:\n- name: OCPI Token\n  type: token\n  in: header\n  header: Authorization\n  encoding:\n    base64_header_2_2_1_plus: >-\n      OCPI 2.2.1+ introduced Base64 encoding of the token in the Authorization\n      header. The token value in the credentials body is unchanged; only the\n      header representation differs. Configured per connection to match\
  \ the\n      partner platform.\n  handshake:\n    module: Credentials\n    setup: Portal > Settings > Roaming Settings > New Handshake (4-step wizard)\n    methods:\n    - enapi-initiates: partner provides Versions URL + Token A; Enapi initiates\n    - partner-initiates: Enapi provides its Versions URL + Token A; partner initiates\n    enapi_party_id: DE*ENA\n    versions_url_production: https://roaming.enapi.com/ocpi/versions\n    versions_url_staging: https://roaming.staging.enapi.com/ocpi/versions\n  sources:\n  - docs://getting-started/set-up-your-ocpi-handshake-with-enapi\n  - docs://technical-documentation/supported-ocpi-modules-and-capabilities\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enapi/refs/heads/main/authentication/enapi-authentication.yml
summary_line: ocpi-token · 1 scheme
tags:
- Company
- EV Charging
- OCPI
- Roaming
- E-Mobility
- Charge Point Operator
- eMSP
- Electric Vehicle
- CDR Clearing
- Interoperability
- Hub
---
