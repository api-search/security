---
api_key_in:
- header
api_specs:
- filename: rubygems-gems-api-openapi.yml
  format: yaml
  label: RubyGems Gems API
  slug: gems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-gems-api-openapi.yml
- filename: rubygems-api-v2-openapi.yml
  format: yaml
  label: RubyGems API V2
  slug: api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-api-v2-openapi.yml
- filename: rubygems-downloads-api-openapi.yml
  format: yaml
  label: RubyGems Downloads API
  slug: downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-downloads-api-openapi.yml
- filename: rubygems-search-api-openapi.yml
  format: yaml
  label: RubyGems Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-search-api-openapi.yml
- filename: rubygems-activity-api-openapi.yml
  format: yaml
  label: RubyGems Activity API
  slug: activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-activity-api-openapi.yml
- filename: rubygems-webhooks-api-openapi.yml
  format: yaml
  label: RubyGems Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rubygems Authentication
name_suffix: Authentication
oauth_flows: []
overview: RubyGems secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: RubyGems
provider_slug: rubygems
scheme_count: 2
schemes:
- description: RubyGems.org API key passed in the Authorization header.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/rubygems-gems-api-openapi.yml
  - openapi/rubygems-webhooks-api-openapi.yml
  type: apiKey
- description: HTTP Basic authentication using email and password. Used for retrieving API keys and authenticated user profiles.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/rubygems-gems-api-openapi.yml
  type: http
slug: rubygems-authentication
source_filename: rubygems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rubygems-gems-api-openapi.yml, openapi/rubygems-webhooks-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: RubyGems.org API key passed in the Authorization header.\n  sources:\n  - openapi/rubygems-gems-api-openapi.yml\n  - openapi/rubygems-webhooks-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using email and password. Used for retrieving API keys\n    and authenticated user profiles.\n  sources:\n  - openapi/rubygems-gems-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/authentication/rubygems-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Ruby
- Package Manager
- Open Source
- Developer Tools
---
