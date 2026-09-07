---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dentsply-sirona-intraoral-modality-openapi.yml
  format: yaml
  label: Dentsply Sirona Intraoral Imaging Modality API
  slug: dsio-modality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dentsply-sirona/refs/heads/main/openapi/dentsply-sirona-intraoral-modality-openapi.yml
- filename: dentsply-sirona-intraoral-filters-openapi.yml
  format: yaml
  label: Dentsply Sirona Intraoral Imaging Filters API
  slug: dsio-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dentsply-sirona/refs/heads/main/openapi/dentsply-sirona-intraoral-filters-openapi.yml
- filename: dentsply-sirona-intraoral-exposure-openapi.yml
  format: yaml
  label: Intraoral Exposure API
  slug: io-exposure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dentsply-sirona/refs/heads/main/openapi/dentsply-sirona-intraoral-exposure-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dentsply Sirona Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dentsply Sirona secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dentsply Sirona
provider_slug: dentsply-sirona
scheme_count: 2
schemes:
- credential_issuance: '"Application developers who have been approved for use with this API will obtain their API key directly from Dentsply Sirona." There is no self-service key issuance.'
  description: 'HTTP Basic. The provider''s wiki states: "Authenticated requests for the Dentsply Sirona Intraoral Modality API follow the Basic authentication method" and "Use of the Dentsply Sirona Intraoral Modality API requires an API key. The API key serves as the password and, with the user name, provides the necessary credentials."'
  docs: https://github.com/dsimaging/dsio-modality-api/wiki/Authentication
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/dentsply-sirona-intraoral-modality-openapi.yml
  type: http
- description: 'Applied globally by the Intraoral Exposure API spec (top-level `security: [ApiKeyAuth]`). That document is a protocol specification for X-ray generator vendors to implement, so the key is issued by whoever operates the generator service, not by Dentsply Sirona.'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/dentsply-sirona-intraoral-exposure-openapi.yml
  type: apiKey
slug: dentsply-sirona-authentication
source_filename: dentsply-sirona-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: openapi/dentsply-sirona-intraoral-exposure-openapi.yml, openapi/dentsply-sirona-intraoral-modality-openapi.yml\ndocs: https://github.com/dsimaging/dsio-modality-api/wiki/Authentication\nnotes: >-\n  Derived from the three first-party OpenAPI documents Dentsply Sirona Imaging publishes on\n  GitHub, then upgraded from the Modality API wiki authentication page. The DS Core cloud API\n  (api.dscore.com) publishes no public authentication documentation — open.dscore.com requires a\n  partner account before any reference is reachable — so no DS Core scheme is recorded here.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/dentsply-sirona-intraoral-modality-openapi.yml\n  docs: https://github.com/dsimaging/dsio-modality-api/wiki/Authentication\n  description: >-\n    HTTP Basic. The provider's wiki states:\
  \ \"Authenticated requests for the Dentsply Sirona\n    Intraoral Modality API follow the Basic authentication method\" and \"Use of the Dentsply Sirona\n    Intraoral Modality API requires an API key. The API key serves as the password and, with the\n    user name, provides the necessary credentials.\"\n  credential_issuance: >-\n    \"Application developers who have been approved for use with this API will obtain their API key\n    directly from Dentsply Sirona.\" There is no self-service key issuance.\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/dentsply-sirona-intraoral-exposure-openapi.yml\n  description: >-\n    Applied globally by the Intraoral Exposure API spec (top-level `security: [ApiKeyAuth]`).\n    That document is a protocol specification for X-ray generator vendors to implement, so the key\n    is issued by whoever operates the generator service, not by Dentsply Sirona.\nunauthenticated_surfaces:\n- openapi/dentsply-sirona-intraoral-filters-openapi.yml\
  \ declares no securitySchemes; the Filters\n  API is a loopback service on the same workstation as the Modality service.\ngaps:\n- DS Core API (https://api.dscore.com) authentication is not publicly documented; the reference is\n  behind the open.dscore.com partner login.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dentsply-sirona/refs/heads/main/authentication/dentsply-sirona-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- CAD/CAM
- CEREC
- Dental
- DS Core
- Imaging
- Intraoral Imaging
- Lab Management
- Medical Devices
- Practice Management
- Fortune 1000
---
