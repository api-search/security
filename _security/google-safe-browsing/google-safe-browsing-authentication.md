---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-safe-browsing-hashes-api-openapi.yml
  format: yaml
  label: Google Safe Browsing Hashes API
  slug: google-safe-browsing-hashes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-safe-browsing/openapi/google-safe-browsing-hashes-api-openapi.yml
- filename: google-safe-browsing-hashlist-api-openapi.yml
  format: yaml
  label: Google Safe Browsing Hash List API
  slug: google-safe-browsing-hashlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-safe-browsing/openapi/google-safe-browsing-hashlist-api-openapi.yml
- filename: google-safe-browsing-hashlists-api-openapi.yml
  format: yaml
  label: Google Safe Browsing Hash Lists API
  slug: google-safe-browsing-hashlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-safe-browsing/openapi/google-safe-browsing-hashlists-api-openapi.yml
- filename: google-safe-browsing-projects-api-openapi.yml
  format: yaml
  label: Google Safe Browsing Projects API
  slug: google-safe-browsing-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-safe-browsing/openapi/google-safe-browsing-projects-api-openapi.yml
- filename: google-safe-browsing-threatlists-api-openapi.yml
  format: yaml
  label: Google Safe Browsing Threat Lists API
  slug: google-safe-browsing-threatlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-safe-browsing/openapi/google-safe-browsing-threatlists-api-openapi.yml
- filename: google-safe-browsing-uris-api-openapi.yml
  format: yaml
  label: Google Safe Browsing Uris API
  slug: google-safe-browsing-uris-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-safe-browsing/openapi/google-safe-browsing-uris-api-openapi.yml
- filename: google-safe-browsing-urls-api-openapi.yml
  format: yaml
  label: Google Safe Browsing URLs API
  slug: google-safe-browsing-urls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-safe-browsing/openapi/google-safe-browsing-urls-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Google Safe Browsing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Google Safe Browsing secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Google Safe Browsing
provider_slug: google-safe-browsing
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: google-safe-browsing-authentication
source_filename: google-safe-browsing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-safe-browsing/authentication/google-safe-browsing-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Google
- Malware
- Safe Browsing
- Security
- Threats
- URLs
---
