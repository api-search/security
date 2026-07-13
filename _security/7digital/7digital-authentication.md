---
api_key_in:
- query
api_specs:
- filename: 7digital-api-openapi.yml
  format: yaml
  label: 7digital API
  slug: 7digital-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7digital/refs/heads/main/openapi/7digital-api-openapi.yml
- filename: 7digital-streaming-platform-openapi.yml
  format: yaml
  label: MassiveMusic Streaming Platform API
  slug: massivemusic-streaming-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7digital/refs/heads/main/openapi/7digital-streaming-platform-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: 7Digital Authentication
name_suffix: Authentication
oauth_flows: []
overview: 7digital secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 7digital
provider_slug: 7digital
scheme_count: 1
schemes:
- description: 7digital uses OAuth 1.0 signing. Every request MUST include `oauth_consumer_key` as either a query parameter or in the Authorization header. Sensitive operations require a 2-legged or 3-legged signature with a user access token.
  in: query
  name: oauth1
  parameter: oauth_consumer_key
  sources:
  - openapi/7digital-api-openapi.yml
  - openapi/7digital-streaming-platform-openapi.yml
  type: apiKey
slug: 7digital-authentication
source_filename: 7digital-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/7digital-api-openapi.yml, openapi/7digital-streaming-platform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: oauth1\n  type: apiKey\n  in: query\n  parameter: oauth_consumer_key\n  description: 7digital uses OAuth 1.0 signing. Every request MUST include `oauth_consumer_key`\n    as either a query parameter or in the Authorization header. Sensitive operations require\n    a 2-legged or 3-legged signature with a user access token.\n  sources:\n  - openapi/7digital-api-openapi.yml\n  - openapi/7digital-streaming-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/7digital/refs/heads/main/authentication/7digital-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Music
- Streaming
- Licensing
- Catalogue
- B2B
- Royalty Reporting
- Public APIs
---
