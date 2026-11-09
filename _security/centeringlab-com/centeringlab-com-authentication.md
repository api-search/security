---
anonymous_access: false
api_key_in: []
api_specs:
- filename: centeringlab-com-grade-api-openapi.yml
  format: yaml
  label: Centering Lab Grade API
  slug: centeringlab-com-grade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-grade-api-openapi.yml
- filename: centeringlab-com-health-api-openapi.yml
  format: yaml
  label: Centering Lab Health API
  slug: centeringlab-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-health-api-openapi.yml
- filename: centeringlab-com-measure-api-openapi.yml
  format: yaml
  label: Centering Lab Measure API
  slug: centeringlab-com-measure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-measure-api-openapi.yml
- filename: centeringlab-com-openapi-json-api-openapi.yml
  format: yaml
  label: Centering Lab Openapi.json API
  slug: centeringlab-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-openapi-json-api-openapi.yml
- filename: centeringlab-com-standards-api-openapi.yml
  format: yaml
  label: Centering Lab Standards API
  slug: centeringlab-com-standards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-standards-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Centeringlab Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Centering Lab secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Centering Lab
provider_slug: centeringlab-com
scheme_count: 1
schemes:
- bearerFormat: Centering Lab partner key
  description: Optional. Without a partner key, existing public IP quotas apply. Partner keys (prefix clp_) that are unknown, revoked or malformed return 401 INVALID_API_KEY; other Authorization values are ignored.
  name: partnerBearer
  scheme: bearer
  sources:
  - openapi/centeringlab-com-openapi.json
  type: http
slug: centeringlab-com-authentication
source_filename: centeringlab-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/centeringlab-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: partnerBearer\n  type: http\n  scheme: bearer\n  bearerFormat: Centering Lab partner key\n  description: Optional. Without a partner key, existing public IP quotas apply. Partner keys\n    (prefix clp_) that are unknown, revoked or malformed return 401 INVALID_API_KEY; other Authorization\n    values are ignored.\n  sources:\n  - openapi/centeringlab-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/centeringlab-com/authentication/centeringlab-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Cards
- Centering
- Collectors
- Web App
---
