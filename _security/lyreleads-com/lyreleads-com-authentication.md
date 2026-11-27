---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lyreleads-com-openapi.json
  format: json
  label: Lyre Leads API
  slug: lyre-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lyreleads-com/openapi/lyreleads-com-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lyre Leads Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lyre Leads secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lyre Leads
provider_slug: lyreleads-com
scheme_count: 1
schemes:
- description: 'API key from your Account page → API Keys tab, on any plan including Free. Format: lyre_<64 hex chars>. An OAuth access token (lyre_oat_...) from a connected app works the same way.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lyreleads-com-openapi.json
  type: http
slug: lyreleads-com-authentication
source_filename: lyreleads-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/lyreleads-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key from your Account page → API Keys tab, on any plan including Free. Format:\n    lyre_<64 hex chars>. An OAuth access token (lyre_oat_...) from a connected app works the\n    same way.'\n  sources:\n  - openapi/lyreleads-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lyreleads-com/authentication/lyreleads-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Business
- Lead Generation
- Data Enrichment
- Marketing
---
