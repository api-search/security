---
api_key_in: []
api_specs:
- filename: spruce-health-openapi.yml
  format: yaml
  label: Spruce Contacts API
  slug: spruce-health-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-openapi.yml
- filename: spruce-health-openapi.yml
  format: yaml
  label: Spruce Conversations API
  slug: spruce-health-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-openapi.yml
- filename: spruce-health-openapi.yml
  format: yaml
  label: Spruce Messages API
  slug: spruce-health-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-openapi.yml
- filename: spruce-health-openapi.yml
  format: yaml
  label: Spruce Webhooks API
  slug: spruce-health-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spruce Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spruce Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spruce Health
provider_slug: spruce-health
scheme_count: 1
schemes:
- description: Organization API token generated in Settings after Spruce Support enables API access.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/spruce-health-openapi.yml
  type: http
slug: spruce-health-authentication
source_filename: spruce-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spruce-health-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Organization API token generated in Settings after Spruce Support enables API\n    access.\n  sources:\n  - openapi/spruce-health-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/authentication/spruce-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- HIPAA
- Communication
- Secure Messaging
- Telehealth
- Contacts
- Conversations
- Messaging
- Webhooks
- VoIP
---
