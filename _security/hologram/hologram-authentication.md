---
api_key_in: []
api_specs:
- filename: hologram-cellular-links-api-openapi.yml
  format: yaml
  label: Hologram Cellular Links API
  slug: hologram-cellular-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-cellular-links-api-openapi.yml
- filename: hologram-devices-api-openapi.yml
  format: yaml
  label: Hologram Devices API
  slug: hologram-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-devices-api-openapi.yml
- filename: hologram-messaging-api-openapi.yml
  format: yaml
  label: Hologram Messaging API
  slug: hologram-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-messaging-api-openapi.yml
- filename: hologram-plans-api-openapi.yml
  format: yaml
  label: Hologram Plans API
  slug: hologram-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-plans-api-openapi.yml
- filename: hologram-sms-api-openapi.yml
  format: yaml
  label: Hologram SMS API
  slug: hologram-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-sms-api-openapi.yml
- filename: hologram-tags-api-openapi.yml
  format: yaml
  label: Hologram Tags API
  slug: hologram-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-tags-api-openapi.yml
- filename: hologram-usage-api-openapi.yml
  format: yaml
  label: Hologram Usage API
  slug: hologram-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-usage-api-openapi.yml
- filename: hologram-webhooks-api-openapi.yml
  format: yaml
  label: Hologram Webhooks API
  slug: hologram-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hologram Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hologram secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hologram
provider_slug: hologram
scheme_count: 1
schemes:
- description: HTTP Basic authentication. Use the literal username `apikey` and your Hologram API key as the password. The API key may alternatively be supplied as an `apikey` query parameter.
  name: apikeyAuth
  scheme: basic
  sources:
  - openapi/hologram-openapi.yml
  type: http
slug: hologram-authentication
source_filename: hologram-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hologram-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apikeyAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Use the literal username `apikey` and your Hologram\n    API key as the password. The API key may alternatively be supplied as an `apikey` query\n    parameter.\n  sources:\n  - openapi/hologram-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/authentication/hologram-authentication.yml
summary_line: http · 1 scheme
tags:
- IoT
- Cellular
- Connectivity
- SIM
- M2M
---
