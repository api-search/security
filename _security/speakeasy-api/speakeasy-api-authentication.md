---
api_key_in: []
api_specs:
- filename: speakeasy-api-artifacts-api-openapi.yml
  format: yaml
  label: Speakeasy Artifacts API
  slug: speakeasy-api-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-artifacts-api-openapi.yml
- filename: speakeasy-api-auth-api-openapi.yml
  format: yaml
  label: Speakeasy Auth API
  slug: speakeasy-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-auth-api-openapi.yml
- filename: speakeasy-api-codesamples-api-openapi.yml
  format: yaml
  label: Speakeasy CodeSamples API
  slug: speakeasy-api-codesamples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-codesamples-api-openapi.yml
- filename: speakeasy-api-events-api-openapi.yml
  format: yaml
  label: Speakeasy Events API
  slug: speakeasy-api-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-events-api-openapi.yml
- filename: speakeasy-api-github-api-openapi.yml
  format: yaml
  label: Speakeasy Github API
  slug: speakeasy-api-github-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-github-api-openapi.yml
- filename: speakeasy-api-organizations-api-openapi.yml
  format: yaml
  label: Speakeasy Organizations API
  slug: speakeasy-api-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-organizations-api-openapi.yml
- filename: speakeasy-api-publishingtokens-api-openapi.yml
  format: yaml
  label: Speakeasy PublishingTokens API
  slug: speakeasy-api-publishingtokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-publishingtokens-api-openapi.yml
- filename: speakeasy-api-reports-api-openapi.yml
  format: yaml
  label: Speakeasy Reports API
  slug: speakeasy-api-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-reports-api-openapi.yml
- filename: speakeasy-api-schemastore-api-openapi.yml
  format: yaml
  label: Speakeasy SchemaStore API
  slug: speakeasy-api-schemastore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-schemastore-api-openapi.yml
- filename: speakeasy-api-shorturls-api-openapi.yml
  format: yaml
  label: Speakeasy ShortURLs API
  slug: speakeasy-api-shorturls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-shorturls-api-openapi.yml
- filename: speakeasy-api-subscriptions-api-openapi.yml
  format: yaml
  label: Speakeasy Subscriptions API
  slug: speakeasy-api-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-subscriptions-api-openapi.yml
- filename: speakeasy-api-suggest-api-openapi.yml
  format: yaml
  label: Speakeasy Suggest API
  slug: speakeasy-api-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-suggest-api-openapi.yml
- filename: speakeasy-api-workspaces-api-openapi.yml
  format: yaml
  label: Speakeasy Workspaces API
  slug: speakeasy-api-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-workspaces-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Speakeasy Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Speakeasy secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Speakeasy
provider_slug: speakeasy-api
scheme_count: 3
schemes:
- description: The API key for the workspace, passed in the x-api-key header.
  headerName: x-api-key
  in: header
  name: APIKey
  sources:
  - openapi/speakeasy-api-openapi.yaml
  type: apiKey
- description: The workspace identifier, passed in the x-workspace-identifier header.
  headerName: x-workspace-identifier
  in: header
  name: WorkspaceIdentifier
  sources:
  - openapi/speakeasy-api-openapi.yaml
  type: apiKey
- description: 'A Bearer token for the workspace, passed as Authorization: Bearer [example key]'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/speakeasy-api-openapi.yaml
  type: http
slug: speakeasy-api-authentication
source_filename: speakeasy-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/speakeasy-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  headerName: x-api-key\n  description: The API key for the workspace, passed in the x-api-key header.\n  sources:\n  - openapi/speakeasy-api-openapi.yaml\n- name: WorkspaceIdentifier\n  type: apiKey\n  in: header\n  headerName: x-workspace-identifier\n  description: The workspace identifier, passed in the x-workspace-identifier header.\n  sources:\n  - openapi/speakeasy-api-openapi.yaml\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: 'A Bearer token for the workspace, passed as Authorization: Bearer [example key]'\n  sources:\n  - openapi/speakeasy-api-openapi.yaml\nnotes: >-\n  The published Speakeasy OpenAPI lists three interchangeable top-level security\n  schemes (APIKey, WorkspaceIdentifier, Bearer). Workspace API keys and tokens are\n  created and managed via the Workspaces\
  \ API and the Speakeasy dashboard/CLI. The\n  CLI typically authenticates interactively (speakeasy auth) and stores credentials\n  locally rather than requiring you to pass headers by hand.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/authentication/speakeasy-api-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- API Lifecycle
- SDK Generation
- Client Library
- API Design
- Developer Tools
- OpenAPI
- Code Generation
- Terraform
- MCP
- Developer Experience
---
