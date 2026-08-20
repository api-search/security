---
api_key_in:
- query
api_specs:
- filename: library-of-congress-bills-api-openapi.yml
  format: yaml
  label: Library of Congress Bills API
  slug: library-of-congress-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-bills-api-openapi.yml
- filename: library-of-congress-collections-api-openapi.yml
  format: yaml
  label: Library of Congress Collections API
  slug: library-of-congress-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-collections-api-openapi.yml
- filename: library-of-congress-committees-api-openapi.yml
  format: yaml
  label: Library of Congress Committees API
  slug: library-of-congress-committees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-committees-api-openapi.yml
- filename: library-of-congress-congressional-record-api-openapi.yml
  format: yaml
  label: Library of Congress Congressional Record API
  slug: library-of-congress-congressional-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-congressional-record-api-openapi.yml
- filename: library-of-congress-issues-api-openapi.yml
  format: yaml
  label: Library of Congress Issues API
  slug: library-of-congress-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-issues-api-openapi.yml
- filename: library-of-congress-items-api-openapi.yml
  format: yaml
  label: Library of Congress Items API
  slug: library-of-congress-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-items-api-openapi.yml
- filename: library-of-congress-laws-api-openapi.yml
  format: yaml
  label: Library of Congress Laws API
  slug: library-of-congress-laws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-laws-api-openapi.yml
- filename: library-of-congress-members-api-openapi.yml
  format: yaml
  label: Library of Congress Members API
  slug: library-of-congress-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-members-api-openapi.yml
- filename: library-of-congress-pages-api-openapi.yml
  format: yaml
  label: Library of Congress Pages API
  slug: library-of-congress-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-pages-api-openapi.yml
- filename: library-of-congress-resources-api-openapi.yml
  format: yaml
  label: Library of Congress Resources API
  slug: library-of-congress-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-resources-api-openapi.yml
- filename: library-of-congress-search-api-openapi.yml
  format: yaml
  label: Library of Congress Search API
  slug: library-of-congress-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-search-api-openapi.yml
- filename: library-of-congress-titles-api-openapi.yml
  format: yaml
  label: Library of Congress Titles API
  slug: library-of-congress-titles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-titles-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Library Of Congress Authentication
name_suffix: Authentication
oauth_flows: []
overview: Library of Congress secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Library of Congress
provider_slug: library-of-congress
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/library-of-congress-congress-gov-api-openapi.yml
  type: apiKey
slug: library-of-congress-authentication
source_filename: library-of-congress-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/library-of-congress-congress-gov-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/library-of-congress-congress-gov-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/authentication/library-of-congress-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cultural Heritage
- Federal-Government
- Library
- Legislative
- Newspapers
- Search
---
