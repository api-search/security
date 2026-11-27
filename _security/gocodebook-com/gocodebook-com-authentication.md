---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gocodebook-com-jurisdictions-api-openapi.yml
  format: yaml
  label: GoCodebook Jurisdictions API
  slug: gocodebook-com-jurisdictions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gocodebook-com/openapi/gocodebook-com-jurisdictions-api-openapi.yml
- filename: gocodebook-com-search-api-openapi.yml
  format: yaml
  label: GoCodebook Search API
  slug: gocodebook-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gocodebook-com/openapi/gocodebook-com-search-api-openapi.yml
- filename: gocodebook-com-topics-api-openapi.yml
  format: yaml
  label: GoCodebook Topics API
  slug: gocodebook-com-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gocodebook-com/openapi/gocodebook-com-topics-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: GoCodebook Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoCodebook secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GoCodebook
provider_slug: gocodebook-com
scheme_count: 1
schemes:
- description: Optional. gcb_live_… or gcb_test_… keys, created by an organization owner or admin. Without a key, requests run on the free sample tier.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/gocodebook-com-openapi.json
  type: http
slug: gocodebook-com-authentication
source_filename: gocodebook-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/gocodebook-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: Optional. gcb_live_… or gcb_test_… keys, created by an organization owner or\n    admin. Without a key, requests run on the free sample tier.\n  sources:\n  - openapi/gocodebook-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/gocodebook-com/authentication/gocodebook-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Building Codes
- Real Estate Law
- Zoning
- AI Research
- Construction
---
