---
api_key_in: []
api_specs:
- filename: inflection-chat-api-openapi.yml
  format: yaml
  label: Inflection AI Chat API
  slug: inflection-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-chat-api-openapi.yml
- filename: inflection-discovery-api-openapi.yml
  format: yaml
  label: Inflection AI Discovery API
  slug: inflection-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-discovery-api-openapi.yml
- filename: inflection-embeddings-api-openapi.yml
  format: yaml
  label: Inflection AI Embeddings API
  slug: inflection-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-embeddings-api-openapi.yml
- filename: inflection-external-api-openapi.yml
  format: yaml
  label: Inflection AI External API
  slug: inflection-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-external-api-openapi.yml
- filename: inflection-status-api-openapi.yml
  format: yaml
  label: Inflection AI Status API
  slug: inflection-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/openapi/inflection-status-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Inflection Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Inflection AI secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Inflection AI
provider_slug: inflection
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: token
  name: OAuth2PasswordBearer
  sources:
  - openapi/inflection-openapi.json
  type: oauth2
slug: inflection-authentication
source_filename: inflection-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/inflection-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: token\n    scopes: 0\n  sources:\n  - openapi/inflection-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inflection/refs/heads/main/authentication/inflection-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- AI
- LLM
- Personal AI
- Pi
- Foundation Models
- Empathetic AI
---
