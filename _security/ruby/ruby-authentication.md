---
api_key_in:
- header
api_specs:
- filename: rubygems-registry-openapi.yml
  format: yaml
  label: RubyGems.org Registry API v1
  slug: rubygems-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ruby/refs/heads/main/openapi/rubygems-registry-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ruby Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ruby Programming Language and Popular API Gems secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ruby Programming Language and Popular API Gems
provider_slug: ruby
scheme_count: 2
schemes:
- description: RubyGems API key issued in the user account settings.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/rubygems-registry-openapi.yml
  type: apiKey
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/rubygems-registry-openapi.yml
  type: http
slug: ruby-authentication
source_filename: ruby-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rubygems-registry-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: RubyGems API key issued in the user account settings.\n  sources:\n  - openapi/rubygems-registry-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/rubygems-registry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ruby/refs/heads/main/authentication/ruby-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Programming Language
- Ruby
- HTTP
- REST
- API Clients
- Frameworks
- Libraries
- Package Registry
---
