---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: aiogeoprotocol-com-audit-api-openapi.yml
  format: yaml
  label: AIO.GEO Protocol Audit API
  slug: aiogeoprotocol-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiogeoprotocol-com/openapi/aiogeoprotocol-com-audit-api-openapi.yml
- filename: aiogeoprotocol-com-brief-api-openapi.yml
  format: yaml
  label: AIO.GEO Protocol Brief API
  slug: aiogeoprotocol-com-brief-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiogeoprotocol-com/openapi/aiogeoprotocol-com-brief-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: AIO.GEO Protocol Authentication
name_suffix: Authentication
oauth_flows: []
overview: AIO.GEO Protocol secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AIO.GEO Protocol
provider_slug: aiogeoprotocol-com
scheme_count: 1
schemes:
- description: Optional ag_live_* key for higher rate limits
  in: header
  name: ApiKeyAuth
  parameter: X-AIO-GEO-Key
  sources:
  - openapi/aiogeoprotocol-com-openapi.json
  type: apiKey
slug: aiogeoprotocol-com-authentication
source_filename: aiogeoprotocol-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/aiogeoprotocol-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-AIO-GEO-Key\n  description: Optional ag_live_* key for higher rate limits\n  sources:\n  - openapi/aiogeoprotocol-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/aiogeoprotocol-com/authentication/aiogeoprotocol-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Search
- Audit
- Measurements
- CLI
---
