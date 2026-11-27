---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gondola-ai-infrastructure-api-openapi.yml
  format: yaml
  label: Gondola Infrastructure API
  slug: gondola-ai-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gondola-ai/openapi/gondola-ai-infrastructure-api-openapi.yml
- filename: gondola-ai-partner-search-api-openapi.yml
  format: yaml
  label: Gondola Partner Search API
  slug: gondola-ai-partner-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gondola-ai/openapi/gondola-ai-partner-search-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Gondola Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gondola secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gondola
provider_slug: gondola-ai
scheme_count: 1
schemes:
- name: PartnerBearer
  scheme: bearer
  sources:
  - openapi/gondola-ai-openapi.json
  type: http
slug: gondola-ai-authentication
source_filename: gondola-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/gondola-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: PartnerBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/gondola-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/gondola-ai/authentication/gondola-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Travel
- Rewards
- Hotel Booking
- Fintech
- Consumer
---
