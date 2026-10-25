---
anonymous_access: false
api_key_in: []
api_specs:
- filename: xylem-docview-api-openapi.yml
  format: yaml
  label: Xylem Doc View API
  slug: xylem-docview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-docview-api-openapi.yml
- filename: xylem-infor-api-openapi.yml
  format: yaml
  label: Xylem Infor API
  slug: xylem-infor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-infor-api-openapi.yml
- filename: xylem-mes-api-openapi.yml
  format: yaml
  label: Xylem MES API
  slug: xylem-mes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-mes-api-openapi.yml
- filename: xylem-mes-v2-api-openapi.yml
  format: yaml
  label: Xylem MES V2 API
  slug: xylem-mes-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-mes-v2-api-openapi.yml
- filename: xylem-nameplate-api-openapi.yml
  format: yaml
  label: Xylem Name Plate API
  slug: xylem-nameplate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-nameplate-api-openapi.yml
- filename: xylem-serialcard-api-openapi.yml
  format: yaml
  label: Xylem Serial Card API
  slug: xylem-serialcard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/openapi/xylem-serialcard-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Xylem Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Xylem secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Xylem
provider_slug: xylem
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: /token
  name: Apis Manager
  sources:
  - openapi/xylem-apis-manager-openapi.yml
  type: oauth2
slug: xylem-authentication
source_filename: xylem-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: derived\nsource: openapi/xylem-apis-manager-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: Apis Manager\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /token\n    scopes: 0\n  sources:\n  - openapi/xylem-apis-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/authentication/xylem-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fortune 1000
- Water
- Water Technology
- Utilities
- Smart Metering
- Industrial IoT
- Water Quality
- Wastewater
- Manufacturing
---
