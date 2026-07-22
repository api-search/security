---
api_key_in:
- header
api_specs:
- filename: unito-embeds-openapi-original.json
  format: json
  label: Unito Embed API
  slug: unito-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unito/refs/heads/main/openapi/unito-embeds-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Unito Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unito secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unito
provider_slug: unito
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/unito-embeds-openapi-original.json
  type: apiKey
slug: unito-authentication
source_filename: unito-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/unito-embeds-openapi-original.json\ndocs: https://dev.unito.io/docs/embeds/embedApi/\nnotes: The Embed API docs confirm API requests are authenticated by an API key passed\n  in the X-API-Key header on each request; keys are issued by Unito per embed entity.\n  The connector platform separately delivers customer credentials to connectors via\n  the X-Unito-Credentials header (custom API key/username+password forms or OAuth2\n  authorizations defined in the connector configuration).\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/unito-embeds-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unito/refs/heads/main/authentication/unito-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Integration
- Two-Way Sync
- Workflow Automation
- Project Management
- Collaboration
- Embedded Integrations
- SaaS
---
