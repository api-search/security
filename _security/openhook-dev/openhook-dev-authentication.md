---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openhook-dev-channel-files-api-openapi.yml
  format: yaml
  label: Openhook Channel Files API
  slug: openhook-dev-channel-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openhook-dev/openapi/openhook-dev-channel-files-api-openapi.yml
- filename: openhook-dev-channels-api-openapi.yml
  format: yaml
  label: Openhook Channels API
  slug: openhook-dev-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openhook-dev/openapi/openhook-dev-channels-api-openapi.yml
- filename: openhook-dev-health-api-openapi.yml
  format: yaml
  label: Openhook Health API
  slug: openhook-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openhook-dev/openapi/openhook-dev-health-api-openapi.yml
- filename: openhook-dev-tools-api-openapi.yml
  format: yaml
  label: Openhook Tools API
  slug: openhook-dev-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openhook-dev/openapi/openhook-dev-tools-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Openhook Authentication
name_suffix: Authentication
oauth_flows: []
overview: Openhook secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Openhook
provider_slug: openhook-dev
scheme_count: 1
schemes:
- description: Your existing private ohp_ channel member key.
  name: MemberKey
  scheme: bearer
  sources:
  - openapi/openhook-dev-openapi.json
  type: http
slug: openhook-dev-authentication
source_filename: openhook-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/openhook-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: MemberKey\n  type: http\n  scheme: bearer\n  description: Your existing private ohp_ channel member key.\n  sources:\n  - openapi/openhook-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/openhook-dev/authentication/openhook-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- Relay
- Open Source
- Private channel
---
