---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: lots-directory-lotsdirectory-api-openapi.yml
  format: yaml
  label: LotsDirectory Lotsdirectory API
  slug: lots-directory-lotsdirectory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lots-directory/openapi/lots-directory-lotsdirectory-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: LotsDirectory Authentication
name_suffix: Authentication
oauth_flows: []
overview: LotsDirectory secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LotsDirectory
provider_slug: lots-directory
scheme_count: 1
schemes:
- description: 'API key for authentication. Format: REDACTED_STRIPE_KEY'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/lots-directory-openapi.yml
  type: apiKey
slug: lots-directory-authentication
source_filename: lots-directory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/lots-directory-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'API key for authentication. Format: REDACTED_STRIPE_KEY'\n  sources:\n  - openapi/lots-directory-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/lots-directory/authentication/lots-directory-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Directories
- Product Launch
- SEO
- Software-as-a-Service
- Launches
---
