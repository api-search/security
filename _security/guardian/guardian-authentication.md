---
api_key_in:
- query
api_specs:
- filename: guardian-content-api-openapi.yml
  format: yaml
  label: The Guardian Content API
  slug: guardian-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardian/refs/heads/main/openapi/guardian-content-api-openapi.yml
- filename: guardian-editions-api-openapi.yml
  format: yaml
  label: The Guardian Editions API
  slug: guardian-editions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardian/refs/heads/main/openapi/guardian-editions-api-openapi.yml
- filename: guardian-sections-api-openapi.yml
  format: yaml
  label: The Guardian Sections API
  slug: guardian-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardian/refs/heads/main/openapi/guardian-sections-api-openapi.yml
- filename: guardian-tags-api-openapi.yml
  format: yaml
  label: The Guardian Tags API
  slug: guardian-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardian/refs/heads/main/openapi/guardian-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Guardian Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Guardian secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Guardian
provider_slug: guardian
scheme_count: 1
schemes:
- description: API key obtained from https://open-platform.theguardian.com/access/. A test key 'test' is available for development.
  in: query
  name: apiKeyQuery
  parameter: api-key
  sources:
  - openapi/openapi.json
  type: apiKey
slug: guardian-authentication
source_filename: guardian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api-key\n  description: API key obtained from https://open-platform.theguardian.com/access/. A test key\n    'test' is available for development.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guardian/refs/heads/main/authentication/guardian-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- News
- Media
- Content
- Articles
- Journalism
---
