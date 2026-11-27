---
anonymous_access: false
api_key_in: []
api_specs:
- filename: elnora-ai-account-api-openapi.yml
  format: yaml
  label: Elnora AI Account API
  slug: elnora-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-account-api-openapi.yml
- filename: elnora-ai-audit-api-openapi.yml
  format: yaml
  label: Elnora AI Audit API
  slug: elnora-ai-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-audit-api-openapi.yml
- filename: elnora-ai-connectionsoauth-api-openapi.yml
  format: yaml
  label: Elnora AI Connections O Auth API
  slug: elnora-ai-connectionsoauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-connectionsoauth-api-openapi.yml
- filename: elnora-ai-feedback-api-openapi.yml
  format: yaml
  label: Elnora AI Feedback API
  slug: elnora-ai-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-feedback-api-openapi.yml
- filename: elnora-ai-files-api-openapi.yml
  format: yaml
  label: Elnora AI Files API
  slug: elnora-ai-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-files-api-openapi.yml
- filename: elnora-ai-folders-api-openapi.yml
  format: yaml
  label: Elnora AI Folders API
  slug: elnora-ai-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-folders-api-openapi.yml
- filename: elnora-ai-mcpconnections-api-openapi.yml
  format: yaml
  label: Elnora AI MCP Connections API
  slug: elnora-ai-mcpconnections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-mcpconnections-api-openapi.yml
- filename: elnora-ai-organization-api-openapi.yml
  format: yaml
  label: Elnora AI Organization API
  slug: elnora-ai-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-organization-api-openapi.yml
- filename: elnora-ai-organizationinvitation-api-openapi.yml
  format: yaml
  label: Elnora AI Organization Invitation API
  slug: elnora-ai-organizationinvitation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-organizationinvitation-api-openapi.yml
- filename: elnora-ai-organizationlibrary-api-openapi.yml
  format: yaml
  label: Elnora AI Organization Library API
  slug: elnora-ai-organizationlibrary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-organizationlibrary-api-openapi.yml
- filename: elnora-ai-publicinvitation-api-openapi.yml
  format: yaml
  label: Elnora AI Public Invitation API
  slug: elnora-ai-publicinvitation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-publicinvitation-api-openapi.yml
- filename: elnora-ai-search-api-openapi.yml
  format: yaml
  label: Elnora AI Search API
  slug: elnora-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-search-api-openapi.yml
- filename: elnora-ai-tasks-api-openapi.yml
  format: yaml
  label: Elnora AI Tasks API
  slug: elnora-ai-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-tasks-api-openapi.yml
- filename: elnora-ai-version-api-openapi.yml
  format: yaml
  label: Elnora AI Version API
  slug: elnora-ai-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-version-api-openapi.yml
- filename: elnora-ai-api-key-api-openapi.yml
  format: yaml
  label: Elnora AI API Key API
  slug: elnora-ai-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elnora-ai/openapi/elnora-ai-api-key-api-openapi.yml
auth_types: []
description: Authentication schemes for Elnora API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Elnora AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elnora AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Elnora AI
provider_slug: elnora-ai
scheme_count: 2
schemes:
- evidence: 'Send it in the X-API-Key header on every request (or as Authorization: Bearer <your-key> — both work)'
  header: X-API-Key
  location: header
  name: X-API-Key
  type: apiKey
- evidence: Interactive clients — including the MCP server — can authenticate with OAuth 2.1.
  name: OAuth 2.1
  type: oauth2
slug: elnora-ai-authentication
source_filename: elnora-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.elnora.ai/docs/get-started/authentication
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.elnora.ai/docs/get-started/authentication\nsources:\n- https://docs.elnora.ai/docs/get-started/authentication\n- https://docs.elnora.ai/docs/api/reference/api-keys\n- https://docs.elnora.ai/docs/cli/api-keys\n- https://docs.elnora.ai/docs/mcp/api-keys.md\ndescription: Authentication schemes for Elnora API\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Send it in the X-API-Key header on every request (or as Authorization: Bearer <your-key> — both work)'\n  location: header\n  header: X-API-Key\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Interactive clients — including the MCP server — can authenticate with OAuth 2.1.\ndocs: https://docs.elnora.ai/docs/get-started/authentication\n"
source_yaml_url: https://artifacts.apis.io/elnora-ai/authentication/elnora-ai-authentication.yml
summary_line: 2 schemes
tags:
- AI Agents
- Lab Automation
- Life Sciences
- Pharma
- CRO
- Research Tools
---
