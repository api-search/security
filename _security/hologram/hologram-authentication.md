---
api_key_in: []
api_specs:
- filename: hologram-openapi.yml
  format: yaml
  label: Hologram Devices & SIMs API
  slug: hologram-devices-sims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-openapi.yml
- filename: hologram-openapi.yml
  format: yaml
  label: Hologram Data Usage API
  slug: hologram-data-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-openapi.yml
- filename: hologram-openapi.yml
  format: yaml
  label: Hologram SMS & Messaging API
  slug: hologram-sms-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-openapi.yml
- filename: hologram-openapi.yml
  format: yaml
  label: Hologram Plans API
  slug: hologram-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-openapi.yml
- filename: hologram-openapi.yml
  format: yaml
  label: Hologram Tags API
  slug: hologram-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-openapi.yml
- filename: hologram-openapi.yml
  format: yaml
  label: Hologram Webhooks API
  slug: hologram-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-openapi.yml
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
