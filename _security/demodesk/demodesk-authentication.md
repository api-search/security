---
api_key_in:
- header
api_specs:
- filename: demodesk-v2-openapi.yml
  format: yaml
  label: Demodesk Public API (v2)
  slug: demodesk-public-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demodesk/refs/heads/main/openapi/demodesk-v2-openapi.yml
- filename: demodesk-v1-openapi.json
  format: json
  label: Demodesk API V1 (deprecated)
  slug: demodesk-api-v1-deprecated
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demodesk/refs/heads/main/openapi/demodesk-v1-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Demodesk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Demodesk secures its APIs with apiKey, http, and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Demodesk
provider_slug: demodesk
scheme_count: 2
schemes:
- in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/demodesk-v1-openapi.json
  type: apiKey
- bearerFormat: API key or OAuth token
  description: 'Pass your API key or OAuth token as a Bearer token in the `Authorization` HTTP header.


    ```

    curl -H "Authorization: Bearer [example key]" https://demodesk.com/api/v2/recordings

    ```


    **Obtaining a key:** Generate an API key in your Demodesk account under

    *Settings > Integrations > Other*.


    **Permissions:** The key inherits the permissions of the user who created it.

    So when trying to access resource'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/demodesk-v2-openapi.yml
  type: http
slug: demodesk-authentication
source_filename: demodesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/demodesk-v1-openapi.json, openapi/demodesk-v2-openapi.yml\ndocs: https://demodesk.com/api/docs/index.html\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_note: >-\n    OAuth2 (authorization_code + PKCE S256, scope mcp:tools) backs the hosted MCP\n    server at https://demodesk.com/mcp. See scopes/demodesk-scopes.yml and\n    well-known/demodesk-oauth-authorization-server.json. The REST API itself uses\n    Bearer API keys.\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/demodesk-v1-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key or OAuth token\n  description: |-\n    Pass your API key or OAuth token as a Bearer token in the `Authorization` HTTP header.\n\n    ```\n    curl -H \"Authorization: Bearer [example key]\" https://demodesk.com/api/v2/recordings\n    ```\n\n    **Obtaining\
  \ a key:** Generate an API key in your Demodesk account under\n    *Settings > Integrations > Other*.\n\n    **Permissions:** The key inherits the permissions of the user who created it.\n    So when trying to access resource\n  sources:\n  - openapi/demodesk-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demodesk/refs/heads/main/authentication/demodesk-authentication.yml
summary_line: apiKey/http/oauth2 · 2 schemes
tags:
- Company
- Sales
- AI
- Conversation Intelligence
- Video Conferencing
- CRM
- Transcription
- Webhooks
- MCP
---
