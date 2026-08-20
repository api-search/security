---
api_key_in:
- query
api_specs:
- filename: sendhub-authentication-api-openapi.yml
  format: yaml
  label: SendHub Authentication API
  slug: sendhub-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendhub/refs/heads/main/openapi/sendhub-authentication-api-openapi.yml
- filename: sendhub-contact-api-openapi.yml
  format: yaml
  label: SendHub Contact API
  slug: sendhub-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendhub/refs/heads/main/openapi/sendhub-contact-api-openapi.yml
- filename: sendhub-group-api-openapi.yml
  format: yaml
  label: SendHub Group API
  slug: sendhub-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendhub/refs/heads/main/openapi/sendhub-group-api-openapi.yml
- filename: sendhub-message-api-openapi.yml
  format: yaml
  label: SendHub Message API
  slug: sendhub-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendhub/refs/heads/main/openapi/sendhub-message-api-openapi.yml
- filename: sendhub-profile-api-openapi.yml
  format: yaml
  label: SendHub Profile API
  slug: sendhub-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendhub/refs/heads/main/openapi/sendhub-profile-api-openapi.yml
- filename: sendhub-thread-api-openapi.yml
  format: yaml
  label: SendHub Thread API
  slug: sendhub-thread-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendhub/refs/heads/main/openapi/sendhub-thread-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sendhub Authentication
name_suffix: Authentication
oauth_flows: []
overview: SendHub secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SendHub
provider_slug: sendhub
scheme_count: 3
schemes:
- description: Your SendHub line's username (can be found in your My Settings page)
  in: query
  name: username
  parameter: username
  sources:
  - openapi/sendhub-authentication-api-openapi.yml
  - openapi/sendhub-contact-api-openapi.yml
  - openapi/sendhub-group-api-openapi.yml
  - openapi/sendhub-message-api-openapi.yml
  - openapi/sendhub-profile-api-openapi.yml
  - openapi/sendhub-thread-api-openapi.yml
  type: apiKey
- description: Your SendHub line's API key (can be found in your My Settings page)
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/sendhub-authentication-api-openapi.yml
  - openapi/sendhub-contact-api-openapi.yml
  - openapi/sendhub-group-api-openapi.yml
  - openapi/sendhub-message-api-openapi.yml
  - openapi/sendhub-profile-api-openapi.yml
  - openapi/sendhub-thread-api-openapi.yml
  type: apiKey
- description: Use your SendHub line's password or API key as the password with HTTP Basic Authentication (Your username and API key can be found in your My Settings page)
  name: basic_auth
  scheme: basic
  sources:
  - openapi/sendhub-authentication-api-openapi.yml
  - openapi/sendhub-contact-api-openapi.yml
  - openapi/sendhub-group-api-openapi.yml
  - openapi/sendhub-message-api-openapi.yml
  - openapi/sendhub-profile-api-openapi.yml
  - openapi/sendhub-thread-api-openapi.yml
  type: http
slug: sendhub-authentication
source_filename: sendhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/sendhub-authentication-api-openapi.yml, openapi/sendhub-contact-api-openapi.yml,\n  openapi/sendhub-group-api-openapi.yml, openapi/sendhub-message-api-openapi.yml, openapi/sendhub-profile-api-openapi.yml,\n  openapi/sendhub-thread-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: username\n  type: apiKey\n  in: query\n  parameter: username\n  description: Your SendHub line's username (can be found in your My Settings page)\n  sources:\n  - openapi/sendhub-authentication-api-openapi.yml\n  - openapi/sendhub-contact-api-openapi.yml\n  - openapi/sendhub-group-api-openapi.yml\n  - openapi/sendhub-message-api-openapi.yml\n  - openapi/sendhub-profile-api-openapi.yml\n  - openapi/sendhub-thread-api-openapi.yml\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Your SendHub line's API key (can be found in your My Settings page)\n  sources:\n\
  \  - openapi/sendhub-authentication-api-openapi.yml\n  - openapi/sendhub-contact-api-openapi.yml\n  - openapi/sendhub-group-api-openapi.yml\n  - openapi/sendhub-message-api-openapi.yml\n  - openapi/sendhub-profile-api-openapi.yml\n  - openapi/sendhub-thread-api-openapi.yml\n- name: basic_auth\n  type: http\n  scheme: basic\n  description: Use your SendHub line's password or API key as the password with HTTP Basic Authentication\n    (Your username and API key can be found in your My Settings page)\n  sources:\n  - openapi/sendhub-authentication-api-openapi.yml\n  - openapi/sendhub-contact-api-openapi.yml\n  - openapi/sendhub-group-api-openapi.yml\n  - openapi/sendhub-message-api-openapi.yml\n  - openapi/sendhub-profile-api-openapi.yml\n  - openapi/sendhub-thread-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendhub/refs/heads/main/authentication/sendhub-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- SMS
- Messaging
- Text Messaging
- Communications
- Marketing
- Webhook
- VoIP
---
