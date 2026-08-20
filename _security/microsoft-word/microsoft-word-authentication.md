---
api_key_in: []
api_specs:
- filename: microsoft-word-body-api-openapi.yml
  format: yaml
  label: Microsoft Word Body API
  slug: microsoft-word-body-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-body-api-openapi.yml
- filename: microsoft-word-checkout-api-openapi.yml
  format: yaml
  label: Microsoft Word Checkout API
  slug: microsoft-word-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-checkout-api-openapi.yml
- filename: microsoft-word-comments-api-openapi.yml
  format: yaml
  label: Microsoft Word Comments API
  slug: microsoft-word-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-comments-api-openapi.yml
- filename: microsoft-word-content-api-openapi.yml
  format: yaml
  label: Microsoft Word Content API
  slug: microsoft-word-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-content-api-openapi.yml
- filename: microsoft-word-content-controls-api-openapi.yml
  format: yaml
  label: Microsoft Word Content Controls API
  slug: microsoft-word-content-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-content-controls-api-openapi.yml
- filename: microsoft-word-documents-api-openapi.yml
  format: yaml
  label: Microsoft Word Documents API
  slug: microsoft-word-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-documents-api-openapi.yml
- filename: microsoft-word-drive-items-api-openapi.yml
  format: yaml
  label: Microsoft Word Drive Items API
  slug: microsoft-word-drive-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-drive-items-api-openapi.yml
- filename: microsoft-word-headers-and-footers-api-openapi.yml
  format: yaml
  label: Microsoft Word Headers And Footers API
  slug: microsoft-word-headers-and-footers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-headers-and-footers-api-openapi.yml
- filename: microsoft-word-images-api-openapi.yml
  format: yaml
  label: Microsoft Word Images API
  slug: microsoft-word-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-images-api-openapi.yml
- filename: microsoft-word-paragraphs-api-openapi.yml
  format: yaml
  label: Microsoft Word Paragraphs API
  slug: microsoft-word-paragraphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-paragraphs-api-openapi.yml
- filename: microsoft-word-permissions-api-openapi.yml
  format: yaml
  label: Microsoft Word Permissions API
  slug: microsoft-word-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-permissions-api-openapi.yml
- filename: microsoft-word-properties-api-openapi.yml
  format: yaml
  label: Microsoft Word Properties API
  slug: microsoft-word-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-properties-api-openapi.yml
- filename: microsoft-word-search-api-openapi.yml
  format: yaml
  label: Microsoft Word Search API
  slug: microsoft-word-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-search-api-openapi.yml
- filename: microsoft-word-sections-api-openapi.yml
  format: yaml
  label: Microsoft Word Sections API
  slug: microsoft-word-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-sections-api-openapi.yml
- filename: microsoft-word-styles-api-openapi.yml
  format: yaml
  label: Microsoft Word Styles API
  slug: microsoft-word-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-styles-api-openapi.yml
- filename: microsoft-word-tables-api-openapi.yml
  format: yaml
  label: Microsoft Word Tables API
  slug: microsoft-word-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-tables-api-openapi.yml
- filename: microsoft-word-thumbnails-api-openapi.yml
  format: yaml
  label: Microsoft Word Thumbnails API
  slug: microsoft-word-thumbnails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-thumbnails-api-openapi.yml
- filename: microsoft-word-versions-api-openapi.yml
  format: yaml
  label: Microsoft Word Versions API
  slug: microsoft-word-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/openapi/microsoft-word-versions-api-openapi.yml
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
- Microsoft-365
- Office
- Productivity
- Word Processing
---
