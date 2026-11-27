---
anonymous_access: false
api_key_in: []
api_specs:
- filename: instabids-ai-drafts-api-openapi.yml
  format: yaml
  label: InstaBids Drafts API
  slug: instabids-ai-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instabids-ai/openapi/instabids-ai-drafts-api-openapi.yml
- filename: instabids-ai-jobs-api-openapi.yml
  format: yaml
  label: InstaBids Jobs API
  slug: instabids-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instabids-ai/openapi/instabids-ai-jobs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: InstaBids Authentication
name_suffix: Authentication
oauth_flows: []
overview: InstaBids secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: InstaBids
provider_slug: instabids-ai
scheme_count: 1
schemes:
- description: A personal InstaBids agent key (ibk_...), created by the homeowner in InstaBids. Limits are per key.
  name: agentKey
  scheme: bearer
  sources:
  - openapi/instabids-ai-dev-openapi.json
  - openapi/instabids-ai-openapi.json
  type: http
slug: instabids-ai-authentication
source_filename: instabids-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/instabids-ai-dev-openapi.json, openapi/instabids-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: agentKey\n  type: http\n  scheme: bearer\n  description: A personal InstaBids agent key (ibk_...), created by the homeowner in InstaBids.\n    Limits are per key.\n  sources:\n  - openapi/instabids-ai-dev-openapi.json\n  - openapi/instabids-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/instabids-ai/authentication/instabids-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Homeowners
- Contractors
- Artificial Intelligence
- Bidding
- Construction
---
