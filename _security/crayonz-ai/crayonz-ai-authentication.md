---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: crayonz-ai-design-pipeline-api-openapi.yml
  format: yaml
  label: Crayonz Design Pipeline API
  slug: crayonz-ai-design-pipeline-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crayonz-ai/openapi/crayonz-ai-design-pipeline-api-openapi.yml
- filename: crayonz-ai-designs-api-openapi.yml
  format: yaml
  label: Crayonz Designs API
  slug: crayonz-ai-designs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crayonz-ai/openapi/crayonz-ai-designs-api-openapi.yml
- filename: crayonz-ai-photoshoot-api-openapi.yml
  format: yaml
  label: Crayonz Photoshoot API
  slug: crayonz-ai-photoshoot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crayonz-ai/openapi/crayonz-ai-photoshoot-api-openapi.yml
- filename: crayonz-ai-virtual-try-on-api-openapi.yml
  format: yaml
  label: Crayonz Virtual Try-On API
  slug: crayonz-ai-virtual-try-on-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crayonz-ai/openapi/crayonz-ai-virtual-try-on-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Crayonz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crayonz secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crayonz
provider_slug: crayonz-ai
scheme_count: 1
schemes:
- alternate: 'Authorization: Bearer <key> (docs: "Send the key as X-API-Key (or Authorization: Bearer )")'
  description: API key prefixed cz_live_ (production) or cz_test_ (sandbox).
  in: header
  key_management: Keys are shown once at creation and stored as a salted hash; rotate or revoke from the console at any time; an expiry date can be set per key (console at https://crayonz.ai/api-console/keys).
  key_prefixes:
    cz_live_: spends real credits and hits real render pipelines
    cz_test_: free, unmetered, returns realistic fixtures instead of calling the image models
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/crayonz-ai-openapi.yml
  - https://crayonz.ai/api/docs
  type: apiKey
slug: crayonz-ai-authentication
source_filename: crayonz-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://crayonz.ai/api/docs\ndocs: https://crayonz.ai/api/docs\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key prefixed cz_live_ (production) or cz_test_ (sandbox).\n  alternate: 'Authorization: Bearer <key> (docs: \"Send the key as X-API-Key (or Authorization: Bearer )\")'\n  key_prefixes:\n    cz_live_: spends real credits and hits real render pipelines\n    cz_test_: free, unmetered, returns realistic fixtures instead of calling the image models\n  key_management: Keys are shown once at creation and stored as a salted hash; rotate or revoke from the console at any time; an expiry date can be set per key (console at https://crayonz.ai/api-console/keys).\n  sources:\n  - openapi/crayonz-ai-openapi.yml\n  - https://crayonz.ai/api/docs\nkey_scopes:\n  note: The docs show API keys carry per-route scopes (not\
  \ OAuth scopes). A key lacking the route's scope gets 403. Only these two scope names are published as examples; no full scope reference was found.\n  examples:\n  - design-api:write\n  - vto:write\n"
source_yaml_url: https://artifacts.apis.io/crayonz-ai/authentication/crayonz-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Custom Apparel
- Print on Demand
- Merchandise
- AI Image Generation
- Design
- Marketplace
- E-Commerce
- India
---
