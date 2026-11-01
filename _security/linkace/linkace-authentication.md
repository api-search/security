---
anonymous_access: false
api_key_in: []
api_specs:
- filename: linkace-bulk-api-openapi.yml
  format: yaml
  label: LinkAce Bulk API
  slug: linkace-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-bulk-api-openapi.yml
- filename: linkace-general-api-openapi.yml
  format: yaml
  label: LinkAce General API
  slug: linkace-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-general-api-openapi.yml
- filename: linkace-links-api-openapi.yml
  format: yaml
  label: LinkAce Links API
  slug: linkace-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-links-api-openapi.yml
- filename: linkace-lists-api-openapi.yml
  format: yaml
  label: LinkAce Lists API
  slug: linkace-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-lists-api-openapi.yml
- filename: linkace-notes-api-openapi.yml
  format: yaml
  label: LinkAce Notes API
  slug: linkace-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-notes-api-openapi.yml
- filename: linkace-search-api-openapi.yml
  format: yaml
  label: LinkAce Search API
  slug: linkace-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-search-api-openapi.yml
- filename: linkace-tags-api-openapi.yml
  format: yaml
  label: LinkAce Tags API
  slug: linkace-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-tags-api-openapi.yml
- filename: linkace-trash-api-openapi.yml
  format: yaml
  label: LinkAce Trash API
  slug: linkace-trash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-trash-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Linkace Authentication
name_suffix: Authentication
oauth_flows: []
overview: LinkAce secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LinkAce
provider_slug: linkace
scheme_count: 1
schemes:
- description: API token received from the user settings
  name: api_token
  scheme: bearer
  sources:
  - openapi/LinkAce-API.v2.yaml
  type: http
slug: linkace-authentication
source_filename: linkace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/LinkAce-API.v2.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: api_token\n  type: http\n  scheme: bearer\n  description: API token received from the user settings\n  sources:\n  - openapi/LinkAce-API.v2.yaml\n"
source_yaml_url: https://artifacts.apis.io/linkace/authentication/linkace-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- OpenSource
- Bookmarking
- SelfHosted
- API
---
