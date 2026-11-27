---
anonymous_access: false
api_key_in: []
api_specs:
- filename: orchis-ai-me-api-openapi.yml
  format: yaml
  label: Orchis.ai LLC Me API
  slug: orchis-ai-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orchis-ai/openapi/orchis-ai-me-api-openapi.yml
- filename: orchis-ai-pulls-api-openapi.yml
  format: yaml
  label: Orchis.ai LLC Pulls API
  slug: orchis-ai-pulls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orchis-ai/openapi/orchis-ai-pulls-api-openapi.yml
- filename: orchis-ai-repos-api-openapi.yml
  format: yaml
  label: Orchis.ai LLC Repos API
  slug: orchis-ai-repos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orchis-ai/openapi/orchis-ai-repos-api-openapi.yml
- filename: orchis-ai-search-api-openapi.yml
  format: yaml
  label: Orchis.ai LLC Search API
  slug: orchis-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orchis-ai/openapi/orchis-ai-search-api-openapi.yml
- filename: orchis-ai-stream-api-openapi.yml
  format: yaml
  label: Orchis.ai LLC Stream API
  slug: orchis-ai-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orchis-ai/openapi/orchis-ai-stream-api-openapi.yml
- filename: orchis-ai-users-api-openapi.yml
  format: yaml
  label: Orchis.ai LLC Users API
  slug: orchis-ai-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orchis-ai/openapi/orchis-ai-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Orchis.ai LLC Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orchis.ai LLC secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orchis.ai LLC
provider_slug: orchis-ai
scheme_count: 1
schemes:
- bearerFormat: orc_pat
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/foundry-orchis-ai-openapi.json
  type: http
slug: orchis-ai-authentication
source_filename: orchis-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/foundry-orchis-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: orc_pat\n  sources:\n  - openapi/foundry-orchis-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/orchis-ai/authentication/orchis-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Infrastructure
- Developer Tools
- Open Source
- Privacy
---
