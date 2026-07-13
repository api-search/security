---
api_key_in: []
api_specs:
- filename: packagist-api-openapi.yml
  format: yaml
  label: Packagist API
  slug: packagist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/packagist/refs/heads/main/openapi/packagist-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Packagist Authentication
name_suffix: Authentication
oauth_flows: []
overview: Packagist secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Packagist
provider_slug: packagist
scheme_count: 1
schemes:
- bearerFormat: username:apiToken
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/packagist-api-openapi.yml
  type: http
slug: packagist-authentication
source_filename: packagist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/packagist-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: username:apiToken\n  sources:\n  - openapi/packagist-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packagist/refs/heads/main/authentication/packagist-authentication.yml
summary_line: http · 1 scheme
tags:
- Composer
- PHP
- Package Registry
- Dependency Management
- Open Source
- Developer Tools
- Software Supply Chain
- Security Advisories
---
