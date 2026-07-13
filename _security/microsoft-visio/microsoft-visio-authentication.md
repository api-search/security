---
api_key_in: []
api_specs:
- filename: microsoft-visio-graph-api.yaml
  format: yaml
  label: Microsoft Graph Visio API
  slug: microsoft-graph-visio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/openapi/microsoft-visio-graph-api.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Visio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Visio secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Visio
provider_slug: microsoft-visio
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization using Microsoft Identity Platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-visio-graph-api.yaml
  type: oauth2
slug: microsoft-visio-authentication
source_filename: microsoft-visio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-visio-graph-api.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 2\n  description: OAuth 2.0 authorization using Microsoft Identity Platform\n  sources:\n  - openapi/microsoft-visio-graph-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/authentication/microsoft-visio-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Business Process
- Diagramming
- Flowcharts
- Microsoft 365
- Visualization
---
