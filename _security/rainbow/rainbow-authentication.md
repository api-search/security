---
api_key_in: []
api_specs:
- filename: rainbow-application-openapi.yml
  format: yaml
  label: Rainbow Application Portal API
  slug: rainbow-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbow/refs/heads/main/openapi/rainbow-application-openapi.yml
- filename: rainbow-messaging-openapi.yml
  format: yaml
  label: Rainbow Messaging API
  slug: rainbow-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbow/refs/heads/main/openapi/rainbow-messaging-openapi.yml
- filename: rainbow-contacts-openapi.yml
  format: yaml
  label: Rainbow Contacts API
  slug: rainbow-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbow/refs/heads/main/openapi/rainbow-contacts-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rainbow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rainbow secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rainbow
provider_slug: rainbow
scheme_count: 1
schemes:
- description: Bearer token from OAuth2 token endpoint
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/rainbow-application-openapi.yml
  - openapi/rainbow-contacts-openapi.yml
  - openapi/rainbow-messaging-openapi.yml
  type: http
slug: rainbow-authentication
source_filename: rainbow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rainbow-application-openapi.yml, openapi/rainbow-contacts-openapi.yml, openapi/rainbow-messaging-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token from OAuth2 token endpoint\n  sources:\n  - openapi/rainbow-application-openapi.yml\n  - openapi/rainbow-contacts-openapi.yml\n  - openapi/rainbow-messaging-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainbow/refs/heads/main/authentication/rainbow-authentication.yml
summary_line: http · 1 scheme
tags:
- Communications
- CPaaS
- Chat
- Voice
- Video
- Telephony
- Messaging
- Collaboration
- Unified Communications
---
