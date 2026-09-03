---
api_key_in: []
api_specs:
- filename: agrio-balance-api-openapi.yml
  format: yaml
  label: agrio Balance API
  slug: agrio-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/openapi/agrio-balance-api-openapi.yml
- filename: agrio-crops-api-openapi.yml
  format: yaml
  label: agrio Crops API
  slug: agrio-crops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/openapi/agrio-crops-api-openapi.yml
- filename: agrio-diagnose-api-openapi.yml
  format: yaml
  label: agrio Diagnose API
  slug: agrio-diagnose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/openapi/agrio-diagnose-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Agrio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agrio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agrio
provider_slug: agrio
scheme_count: 1
schemes:
- description: API key obtained from the Agrio API portal at pro.agrio.app/image-diagnosis-api. Include as a Bearer token in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/agrio-openapi-original.yml
  type: http
slug: agrio-authentication
source_filename: agrio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agrio-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key obtained from the Agrio API portal at pro.agrio.app/image-diagnosis-api.\n    Include as a Bearer token in the Authorization header.\n  sources:\n  - openapi/agrio-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/authentication/agrio-authentication.yml
summary_line: http · 1 scheme
tags:
- Agriculture
- Plant Disease
- Pest Detection
- Artificial Intelligence
- Crop Advisory
---
