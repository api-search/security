---
api_key_in: []
api_specs:
- filename: zulip-events-asyncapi.yml
  format: yaml
  label: Zulip REST API
  slug: rest-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/asyncapi/zulip-events-asyncapi.yml
- filename: zulip-events-asyncapi.yml
  format: yaml
  label: Zulip Events API
  slug: events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/asyncapi/zulip-events-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zulip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zulip secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zulip
provider_slug: zulip
scheme_count: 1
schemes:
- description: 'Basic authentication, with the user''s email as the username, and the API

    key as the password. The API key can be fetched using the

    `/fetch_api_key` or `/dev_fetch_api_key` endpoints.'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/zulip-openapi.yml
  type: http
slug: zulip-authentication
source_filename: zulip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zulip-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Basic authentication, with the user's email as the username, and the API\n    key as the password. The API key can be fetched using the\n    `/fetch_api_key` or `/dev_fetch_api_key` endpoints.\n  sources:\n  - openapi/zulip-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/authentication/zulip-authentication.yml
summary_line: http · 1 scheme
tags:
- Collaboration
- Messaging
- Team Chat
- Webhooks
---
