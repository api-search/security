---
api_key_in:
- header
api_specs:
- filename: openhands-add-git-providers-api-openapi.yml
  format: yaml
  label: OpenHands Add Git Providers API
  slug: openhands-add-git-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openhands/refs/heads/main/openapi/openhands-add-git-providers-api-openapi.yml
- filename: openhands-alive-api-openapi.yml
  format: yaml
  label: OpenHands Alive API
  slug: openhands-alive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openhands/refs/heads/main/openapi/openhands-alive-api-openapi.yml
- filename: openhands-conversations-api-openapi.yml
  format: yaml
  label: OpenHands Conversations API
  slug: openhands-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openhands/refs/heads/main/openapi/openhands-conversations-api-openapi.yml
- filename: openhands-health-api-openapi.yml
  format: yaml
  label: OpenHands Health API
  slug: openhands-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openhands/refs/heads/main/openapi/openhands-health-api-openapi.yml
- filename: openhands-options-api-openapi.yml
  format: yaml
  label: OpenHands Options API
  slug: openhands-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openhands/refs/heads/main/openapi/openhands-options-api-openapi.yml
- filename: openhands-reset-settings-api-openapi.yml
  format: yaml
  label: OpenHands Reset Settings API
  slug: openhands-reset-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openhands/refs/heads/main/openapi/openhands-reset-settings-api-openapi.yml
- filename: openhands-secrets-api-openapi.yml
  format: yaml
  label: OpenHands Secrets API
  slug: openhands-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openhands/refs/heads/main/openapi/openhands-secrets-api-openapi.yml
- filename: openhands-settings-api-openapi.yml
  format: yaml
  label: OpenHands Settings API
  slug: openhands-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openhands/refs/heads/main/openapi/openhands-settings-api-openapi.yml
- filename: openhands-unset-provider-tokens-api-openapi.yml
  format: yaml
  label: OpenHands Unset Provider Tokens API
  slug: openhands-unset-provider-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openhands/refs/heads/main/openapi/openhands-unset-provider-tokens-api-openapi.yml
- filename: openhands-user-api-openapi.yml
  format: yaml
  label: OpenHands User API
  slug: openhands-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openhands/refs/heads/main/openapi/openhands-user-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openhands Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenHands secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenHands
provider_slug: openhands
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-Session-API-Key
  sources:
  - openapi/openhands-openapi.json
  type: apiKey
slug: openhands-authentication
source_filename: openhands-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openhands-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Session-API-Key\n  sources:\n  - openapi/openhands-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openhands/refs/heads/main/authentication/openhands-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Agents
- Autonomous
- Open-Source
- Developer Tools
- Software Engineering
- Code Generation
---
