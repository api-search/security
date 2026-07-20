---
api_key_in: []
api_specs:
- filename: microsoft-word-graph-api.yaml
  format: yaml
  label: Microsoft Graph Word API
  slug: microsoft-graph-word-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-graph-api.yaml
- filename: microsoft-word-javascript-api.yaml
  format: yaml
  label: Office JavaScript API for Word
  slug: office-javascript-api-for-word
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-javascript-api.yaml
- filename: microsoft-word-open-xml-sdk.yaml
  format: yaml
  label: Open XML SDK for Word
  slug: open-xml-sdk-for-word
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-open-xml-sdk.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Microsoft Word Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Word secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Word
provider_slug: microsoft-word
scheme_count: 2
schemes:
- description: OAuth 2.0 authorization code flow with Microsoft Identity Platform (delegated).
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-word-graph-api.yaml
  - openapi/microsoft-word-javascript-api.yaml
  type: oauth2
- description: App-only (daemon) access using application permissions and the .default scope (https://graph.microsoft.com/.default). Documented for server-side automation such as Word Automation Services and unattended document processing.
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2-client-credentials
  sources:
  - docs
  type: oauth2
slug: microsoft-word-authentication
source_filename: microsoft-word-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/microsoft-word-graph-api.yaml, openapi/microsoft-word-javascript-api.yaml\ndocs: https://learn.microsoft.com/en-us/graph/auth/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  identity_platform: Microsoft Entra / Microsoft Identity Platform (v2.0 endpoint)\n  token_type: OAuth 2.0 bearer (JWT)\n  consent: delegated permissions (user consent) and application permissions (admin consent)\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 4\n  description: OAuth 2.0 authorization code flow with Microsoft Identity Platform (delegated).\n  sources:\n  - openapi/microsoft-word-graph-api.yaml\n  - openapi/microsoft-word-javascript-api.yaml\n- name: oauth2-client-credentials\n\
  \  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  description: >-\n    App-only (daemon) access using application permissions and the .default scope\n    (https://graph.microsoft.com/.default). Documented for server-side automation such as\n    Word Automation Services and unattended document processing.\n  sources:\n  - docs\ndiscovery:\n  openid_configuration: https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration\n  see: well-known/microsoft-word-well-known.yml\nscopes_artifact: scopes/microsoft-word-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/authentication/microsoft-word-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Documents
- Microsoft 365
- Office
- Productivity
- Word Processing
---
