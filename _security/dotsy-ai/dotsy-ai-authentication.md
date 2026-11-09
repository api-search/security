---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dotsy-ai-account-api-openapi.yml
  format: yaml
  label: dotsy Account API
  slug: dotsy-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-account-api-openapi.yml
- filename: dotsy-ai-assets-api-openapi.yml
  format: yaml
  label: dotsy Assets API
  slug: dotsy-ai-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-assets-api-openapi.yml
- filename: dotsy-ai-brief-api-openapi.yml
  format: yaml
  label: dotsy Brief API
  slug: dotsy-ai-brief-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-brief-api-openapi.yml
- filename: dotsy-ai-collections-api-openapi.yml
  format: yaml
  label: dotsy Collections API
  slug: dotsy-ai-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-collections-api-openapi.yml
- filename: dotsy-ai-content-api-openapi.yml
  format: yaml
  label: dotsy Content API
  slug: dotsy-ai-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-content-api-openapi.yml
- filename: dotsy-ai-domains-api-openapi.yml
  format: yaml
  label: dotsy Domains API
  slug: dotsy-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-domains-api-openapi.yml
- filename: dotsy-ai-draft-publish-api-openapi.yml
  format: yaml
  label: dotsy Draft & publish API
  slug: dotsy-ai-draft-publish-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-draft-publish-api-openapi.yml
- filename: dotsy-ai-forms-api-openapi.yml
  format: yaml
  label: dotsy Forms API
  slug: dotsy-ai-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-forms-api-openapi.yml
- filename: dotsy-ai-guest-api-openapi.yml
  format: yaml
  label: dotsy Guest API
  slug: dotsy-ai-guest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-guest-api-openapi.yml
- filename: dotsy-ai-import-api-openapi.yml
  format: yaml
  label: dotsy Import API
  slug: dotsy-ai-import-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-import-api-openapi.yml
- filename: dotsy-ai-jobs-api-openapi.yml
  format: yaml
  label: dotsy Jobs API
  slug: dotsy-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-jobs-api-openapi.yml
- filename: dotsy-ai-members-api-openapi.yml
  format: yaml
  label: dotsy Members API
  slug: dotsy-ai-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-members-api-openapi.yml
- filename: dotsy-ai-pages-api-openapi.yml
  format: yaml
  label: dotsy Pages API
  slug: dotsy-ai-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-pages-api-openapi.yml
- filename: dotsy-ai-routes-api-openapi.yml
  format: yaml
  label: dotsy Routes API
  slug: dotsy-ai-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-routes-api-openapi.yml
- filename: dotsy-ai-sites-api-openapi.yml
  format: yaml
  label: dotsy Sites API
  slug: dotsy-ai-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-sites-api-openapi.yml
- filename: dotsy-ai-support-api-openapi.yml
  format: yaml
  label: dotsy Support API
  slug: dotsy-ai-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-support-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Dotsy Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: dotsy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: dotsy
provider_slug: dotsy-ai
scheme_count: 1
schemes:
- description: Account API key (pga_…). OAuth MCP sessions use the same header with an opaque token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/dotsy-ai-openapi.yml
  type: http
slug: dotsy-ai-authentication
source_filename: dotsy-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/dotsy-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Account API key (pga_…). OAuth MCP sessions use the same header with an opaque\n    token.\n  sources:\n  - openapi/dotsy-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/dotsy-ai/authentication/dotsy-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Website Builder
- No-Code
- Free
---
