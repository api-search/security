---
api_key_in:
- header
api_specs:
- filename: speakeasy-artifacts-api-openapi.yml
  format: yaml
  label: Speakeasy Artifacts API
  slug: speakeasy-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-artifacts-api-openapi.yml
- filename: speakeasy-auth-api-openapi.yml
  format: yaml
  label: Speakeasy Auth API
  slug: speakeasy-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-auth-api-openapi.yml
- filename: speakeasy-codesamples-api-openapi.yml
  format: yaml
  label: Speakeasy CodeSamples API
  slug: speakeasy-codesamples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-codesamples-api-openapi.yml
- filename: speakeasy-events-api-openapi.yml
  format: yaml
  label: Speakeasy Events API
  slug: speakeasy-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-events-api-openapi.yml
- filename: speakeasy-github-api-openapi.yml
  format: yaml
  label: Speakeasy Github API
  slug: speakeasy-github-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-github-api-openapi.yml
- filename: speakeasy-organizations-api-openapi.yml
  format: yaml
  label: Speakeasy Organizations API
  slug: speakeasy-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-organizations-api-openapi.yml
- filename: speakeasy-publishingtokens-api-openapi.yml
  format: yaml
  label: Speakeasy PublishingTokens API
  slug: speakeasy-publishingtokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-publishingtokens-api-openapi.yml
- filename: speakeasy-reports-api-openapi.yml
  format: yaml
  label: Speakeasy Reports API
  slug: speakeasy-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-reports-api-openapi.yml
- filename: speakeasy-schemastore-api-openapi.yml
  format: yaml
  label: Speakeasy SchemaStore API
  slug: speakeasy-schemastore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-schemastore-api-openapi.yml
- filename: speakeasy-shorturls-api-openapi.yml
  format: yaml
  label: Speakeasy ShortURLs API
  slug: speakeasy-shorturls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-shorturls-api-openapi.yml
- filename: speakeasy-subscriptions-api-openapi.yml
  format: yaml
  label: Speakeasy Subscriptions API
  slug: speakeasy-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-subscriptions-api-openapi.yml
- filename: speakeasy-suggest-api-openapi.yml
  format: yaml
  label: Speakeasy Suggest API
  slug: speakeasy-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-suggest-api-openapi.yml
- filename: speakeasy-workspaces-api-openapi.yml
  format: yaml
  label: Speakeasy Workspaces API
  slug: speakeasy-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-workspaces-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Speakeasy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Speakeasy secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Speakeasy
provider_slug: speakeasy
scheme_count: 3
schemes:
- description: The API Key for the workspace
  in: header
  name: APIKey
  parameter: x-api-key
  sources:
  - openapi/speakeasy-openapi.yml
  type: apiKey
- description: The API Key for the workspace
  in: header
  name: WorkspaceIdentifier
  parameter: x-workspace-identifier
  sources:
  - openapi/speakeasy-openapi.yml
  type: apiKey
- description: The Bearer token for the workspace
  name: Bearer
  scheme: bearer
  sources:
  - openapi/speakeasy-openapi.yml
  type: http
slug: speakeasy-authentication
source_filename: speakeasy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/speakeasy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: The API Key for the workspace\n  sources:\n  - openapi/speakeasy-openapi.yml\n- name: WorkspaceIdentifier\n  type: apiKey\n  in: header\n  parameter: x-workspace-identifier\n  description: The API Key for the workspace\n  sources:\n  - openapi/speakeasy-openapi.yml\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: The Bearer token for the workspace\n  sources:\n  - openapi/speakeasy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/authentication/speakeasy-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- AI
- Documentation
- MCP
- Platform
- SDKs
- Terraform
- Testing
---
