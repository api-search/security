---
api_key_in:
- header
api_specs:
- filename: ortto-accounts-api-openapi.yml
  format: yaml
  label: Ortto Accounts API
  slug: ortto-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-accounts-api-openapi.yml
- filename: ortto-activities-api-openapi.yml
  format: yaml
  label: Ortto Activities API
  slug: ortto-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-activities-api-openapi.yml
- filename: ortto-campaigns-api-openapi.yml
  format: yaml
  label: Ortto Campaigns API
  slug: ortto-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-campaigns-api-openapi.yml
- filename: ortto-people-api-openapi.yml
  format: yaml
  label: Ortto People API
  slug: ortto-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-people-api-openapi.yml
- filename: ortto-tags-api-openapi.yml
  format: yaml
  label: Ortto Tags API
  slug: ortto-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-tags-api-openapi.yml
- filename: ortto-transactional-api-openapi.yml
  format: yaml
  label: Ortto Transactional API
  slug: ortto-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-transactional-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ortto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ortto secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ortto
provider_slug: ortto
scheme_count: 1
schemes:
- description: Custom private API key configured in Ortto under Settings, supplied on every request in the X-Api-Key header.
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/ortto-openapi.yml
  type: apiKey
slug: ortto-authentication
source_filename: ortto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ortto-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Custom private API key configured in Ortto under Settings, supplied on every\n    request in the X-Api-Key header.\n  sources:\n  - openapi/ortto-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/authentication/ortto-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Marketing Automation
- CDP
- Customer Data Platform
- Analytics
- Email
---
