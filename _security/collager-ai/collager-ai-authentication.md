---
anonymous_access: false
api_key_in: []
api_specs:
- filename: collager-ai-account-api-openapi.yml
  format: yaml
  label: Collager.ai Account API
  slug: collager-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/collager-ai/openapi/collager-ai-account-api-openapi.yml
- filename: collager-ai-collages-api-openapi.yml
  format: yaml
  label: Collager.ai Collages API
  slug: collager-ai-collages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/collager-ai/openapi/collager-ai-collages-api-openapi.yml
- filename: collager-ai-mosaics-api-openapi.yml
  format: yaml
  label: Collager.ai Mosaics API
  slug: collager-ai-mosaics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/collager-ai/openapi/collager-ai-mosaics-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Collager.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Collager.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Collager.ai
provider_slug: collager-ai
scheme_count: 1
schemes:
- description: 'API key from https://collager.ai/developers/ : Authorization: Bearer <key>'
  docs_quote: 'Every request carries Authorization: Bearer <key> over HTTPS. A key is bound to one Collager.ai account and spends that account''s credits.'
  guidance: Keep keys on your server — never in a browser or mobile app.
  issuance: Keys issued by hand on request; there is no self-serve free tier.
  key_prefixes:
  - meaning: creates real jobs and can unlock HD files
    prefix: ck_live_
  - meaning: creates jobs that end at a watermarked preview and never spend credits
    prefix: ck_test_
  name: bearerKey
  scheme: bearer
  sources:
  - openapi/collager-ai-openapi.yml
  - https://collager.ai/developers/
  type: http
slug: collager-ai-authentication
source_filename: collager-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://collager.ai/developers/\ndocs: https://collager.ai/developers/\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerKey\n  type: http\n  scheme: bearer\n  description: 'API key from https://collager.ai/developers/ : Authorization: Bearer <key>'\n  key_prefixes:\n  - prefix: ck_live_\n    meaning: creates real jobs and can unlock HD files\n  - prefix: ck_test_\n    meaning: creates jobs that end at a watermarked preview and never spend credits\n  issuance: Keys issued by hand on request; there is no self-serve free tier.\n  docs_quote: \"Every request carries Authorization: Bearer <key> over HTTPS. A key is bound to one Collager.ai account and spends that account's credits.\"\n  guidance: Keep keys on your server — never in a browser or mobile app.\n  sources:\n  - openapi/collager-ai-openapi.yml\n  - https://collager.ai/developers/\nnotes: The MCP server at https://collager.ai/mcp is documented as callable without\
  \ a key.\n"
source_yaml_url: https://artifacts.apis.io/collager-ai/authentication/collager-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Photo Mosaic
- Photo Collage
- Image Generation
- Artificial Intelligence
- MCP
- Photography
---
