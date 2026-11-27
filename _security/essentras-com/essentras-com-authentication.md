---
anonymous_access: false
api_key_in: []
api_specs:
- filename: essentras-com-agent-api-openapi.yml
  format: yaml
  label: Essentras Agent API
  slug: essentras-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/essentras-com/openapi/essentras-com-agent-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Essentras Authentication
name_suffix: Authentication
oauth_flows: []
overview: Essentras secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Essentras
provider_slug: essentras-com
scheme_count: 1
schemes:
- bearerFormat: ess_live_...
  description: Secret API key from https://essentras.com/account/api. Also accepted in the X-Api-Key header. A key that is sent but invalid is a 401, never a silent fall back to public prices.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/essentras-com-openapi.json
  type: http
slug: essentras-com-authentication
source_filename: essentras-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/essentras-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: ess_live_...\n  description: Secret API key from https://essentras.com/account/api. Also accepted in the X-Api-Key\n    header. A key that is sent but invalid is a 401, never a silent fall back to public prices.\n  sources:\n  - openapi/essentras-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/essentras-com/authentication/essentras-com-authentication.yml
summary_line: http · 1 scheme
tags:
- PR
- Marketplace
- Media
- Artificial Intelligence
- Content Distribution
- Company
---
