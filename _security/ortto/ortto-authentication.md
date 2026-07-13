---
api_key_in:
- header
api_specs:
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto People / Contacts API
  slug: people-contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Custom Activities API
  slug: custom-activities
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Campaigns API
  slug: campaigns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Tags API
  slug: tags
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Transactional Email API
  slug: transactional-email
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
- filename: ortto-openapi.yml
  format: yaml
  label: Ortto Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-openapi.yml
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
