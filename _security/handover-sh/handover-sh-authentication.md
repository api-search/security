---
anonymous_access: false
api_key_in: []
api_specs:
- filename: handover-sh-activity-api-openapi.yml
  format: yaml
  label: 44pixels Limited Activity API
  slug: handover-sh-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-activity-api-openapi.yml
- filename: handover-sh-agents-api-openapi.yml
  format: yaml
  label: 44pixels Limited Agents API
  slug: handover-sh-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-agents-api-openapi.yml
- filename: handover-sh-analytics-api-openapi.yml
  format: yaml
  label: 44pixels Limited Analytics API
  slug: handover-sh-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-analytics-api-openapi.yml
- filename: handover-sh-artifacts-api-openapi.yml
  format: yaml
  label: 44pixels Limited Artifacts API
  slug: handover-sh-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-artifacts-api-openapi.yml
- filename: handover-sh-connectors-api-openapi.yml
  format: yaml
  label: 44pixels Limited Connectors API
  slug: handover-sh-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-connectors-api-openapi.yml
- filename: handover-sh-exports-api-openapi.yml
  format: yaml
  label: 44pixels Limited Exports API
  slug: handover-sh-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-exports-api-openapi.yml
- filename: handover-sh-folders-api-openapi.yml
  format: yaml
  label: 44pixels Limited Folders API
  slug: handover-sh-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-folders-api-openapi.yml
- filename: handover-sh-handovers-api-openapi.yml
  format: yaml
  label: 44pixels Limited Handovers API
  slug: handover-sh-handovers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-handovers-api-openapi.yml
- filename: handover-sh-imports-api-openapi.yml
  format: yaml
  label: 44pixels Limited Imports API
  slug: handover-sh-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-imports-api-openapi.yml
- filename: handover-sh-me-api-openapi.yml
  format: yaml
  label: 44pixels Limited Me API
  slug: handover-sh-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-me-api-openapi.yml
- filename: handover-sh-notifications-api-openapi.yml
  format: yaml
  label: 44pixels Limited Notifications API
  slug: handover-sh-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-notifications-api-openapi.yml
- filename: handover-sh-operations-api-openapi.yml
  format: yaml
  label: 44pixels Limited Operations API
  slug: handover-sh-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-operations-api-openapi.yml
- filename: handover-sh-organization-api-openapi.yml
  format: yaml
  label: 44pixels Limited Organization API
  slug: handover-sh-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-organization-api-openapi.yml
- filename: handover-sh-publications-api-openapi.yml
  format: yaml
  label: 44pixels Limited Publications API
  slug: handover-sh-publications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-publications-api-openapi.yml
- filename: handover-sh-reliability-api-openapi.yml
  format: yaml
  label: 44pixels Limited Reliability API
  slug: handover-sh-reliability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-reliability-api-openapi.yml
- filename: handover-sh-reports-api-openapi.yml
  format: yaml
  label: 44pixels Limited Reports API
  slug: handover-sh-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-reports-api-openapi.yml
- filename: handover-sh-search-api-openapi.yml
  format: yaml
  label: 44pixels Limited Search API
  slug: handover-sh-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-search-api-openapi.yml
- filename: handover-sh-spaces-api-openapi.yml
  format: yaml
  label: 44pixels Limited Spaces API
  slug: handover-sh-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-spaces-api-openapi.yml
- filename: handover-sh-storage-api-openapi.yml
  format: yaml
  label: 44pixels Limited Storage API
  slug: handover-sh-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-storage-api-openapi.yml
- filename: handover-sh-tokens-api-openapi.yml
  format: yaml
  label: 44pixels Limited Tokens API
  slug: handover-sh-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handover-sh/openapi/handover-sh-tokens-api-openapi.yml
auth_types: []
description: Authentication methods for MCP as described in Handover documentation.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: 44pixels Limited Authentication
name_suffix: Authentication
oauth_flows: []
overview: 44pixels Limited declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: 44pixels Limited
provider_slug: handover-sh
scheme_count: 2
schemes:
- evidence: Public clients use authorization code with PKCE, tokens are sent in the Authorization header, and the resource server validates issuer, audience, expiry, and scopes on every request.
  how_to_obtain: Interactive browser‑based authorization flow using PKCE as defined by the MCP authorization specification.
  name: MCP OAuth
  type: oauth2
- evidence: '"Authorization": "Bearer <SERVICE_AGENT_TOKEN>"'
  header: Authorization
  how_to_obtain: Create a named service‑agent in Handover and use its token as a Bearer token in the Authorization header.
  location: header
  name: Service Agent Token
  type: http-bearer
slug: handover-sh-authentication
source_filename: handover-sh-authentication.yml
source_heading: Authentication Profile
source_url: https://handover.sh/guides/mcp-oauth-vs-service-accounts
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://handover.sh/guides/mcp-oauth-vs-service-accounts\nsources:\n- https://handover.sh/guides/mcp-oauth-vs-service-accounts\n- https://handover.sh/guides/cline-mcp-server-setup\n- https://handover.sh/guides/gemini-cli-mcp-server-setup\n- https://handover.sh/guides/claude-code-mcp-server-setup\ndescription: Authentication methods for MCP as described in Handover documentation.\nschemes:\n- type: oauth2\n  name: MCP OAuth\n  evidence: Public clients use authorization code with PKCE, tokens are sent in the Authorization header, and the resource server validates issuer,\n    audience, expiry, and scopes on every request.\n  how_to_obtain: Interactive browser‑based authorization flow using PKCE as defined by the MCP authorization specification.\n- type: http-bearer\n  name: Service Agent Token\n  evidence: '\"Authorization\": \"Bearer <SERVICE_AGENT_TOKEN>\"'\n  location: header\n\
  \  header: Authorization\n  how_to_obtain: Create a named service‑agent in Handover and use its token as a Bearer token in the Authorization header.\ndocs: https://handover.sh/guides/mcp-oauth-vs-service-accounts\n"
source_yaml_url: https://artifacts.apis.io/handover-sh/authentication/handover-sh-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
