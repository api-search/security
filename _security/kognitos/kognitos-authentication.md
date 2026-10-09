---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kognitos-analytics-api-openapi.yml
  format: yaml
  label: Kognitos Analytics API
  slug: kognitos-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-analytics-api-openapi.yml
- filename: kognitos-automations-api-openapi.yml
  format: yaml
  label: Kognitos Automations API
  slug: kognitos-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-automations-api-openapi.yml
- filename: kognitos-books-api-openapi.yml
  format: yaml
  label: Kognitos Books API
  slug: kognitos-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-books-api-openapi.yml
- filename: kognitos-exceptions-api-openapi.yml
  format: yaml
  label: Kognitos Exceptions API
  slug: kognitos-exceptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-exceptions-api-openapi.yml
- filename: kognitos-files-api-openapi.yml
  format: yaml
  label: Kognitos Files API
  slug: kognitos-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-files-api-openapi.yml
- filename: kognitos-organizations-api-openapi.yml
  format: yaml
  label: Kognitos Organizations API
  slug: kognitos-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-organizations-api-openapi.yml
- filename: kognitos-runs-api-openapi.yml
  format: yaml
  label: Kognitos Runs API
  slug: kognitos-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-runs-api-openapi.yml
- filename: kognitos-workspaces-api-openapi.yml
  format: yaml
  label: Kognitos Workspaces API
  slug: kognitos-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/openapi/kognitos-workspaces-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Kognitos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kognitos secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kognitos
provider_slug: kognitos
scheme_count: 2
schemes:
- applies_to: Kognitos REST API (https://app.us-1.kognitos.com/api/v1) and MCP server (non-interactive use)
  description: Personal Access Token (API key) sent in the Authorization header as Bearer YOUR_API_KEY. Created in the Kognitos UI (user menu > API Keys); shown once at creation. Expiration choices are 7 days, 30 days, 60 days, 90 days, 180 days, or 1 year. Each key is scoped to All Workspaces or Specific Workspaces and carries a permission level of All, Read only, or Restricted (custom per-resource permissions). Up to 10 API keys per organization. Deleting a key immediately revokes it.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/kognitos-openapi.yml
  - https://docs.kognitos.com/guides/api-reference/api-reference
  - https://docs.kognitos.com/guides/api-reference/api-keys
  type: http
- applies_to: Kognitos MCP Server only
  description: The MCP server (https://mcp.us-1.kognitos.com/) supports OAuth 2.1 for interactive clients (Claude Desktop, Claude Code, Claude.ai) - browser login and approval, short-lived tokens refreshed by the client, access scoped to the user's account and permissions. Documented as recommended over API keys for interactive clients. No scope list is published.
  name: MCP OAuth 2.1
  sources:
  - https://docs.kognitos.com/guides/mcp/mcp
  type: oauth2
slug: kognitos-authentication
source_filename: kognitos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: https://docs.kognitos.com/guides/api-reference/api-keys\ndocs: https://docs.kognitos.com/guides/api-reference/api-keys\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Personal Access Token (API key) sent in the Authorization header as Bearer YOUR_API_KEY. Created in\n    the Kognitos UI (user menu > API Keys); shown once at creation. Expiration choices are 7 days, 30 days,\n    60 days, 90 days, 180 days, or 1 year. Each key is scoped to All Workspaces or Specific Workspaces and\n    carries a permission level of All, Read only, or Restricted (custom per-resource permissions). Up to\n    10 API keys per organization. Deleting a key immediately revokes it.\n  applies_to: Kognitos REST API (https://app.us-1.kognitos.com/api/v1) and MCP server (non-interactive use)\n  sources:\n  - openapi/kognitos-openapi.yml\n  - https://docs.kognitos.com/guides/api-reference/api-reference\n\
  \  - https://docs.kognitos.com/guides/api-reference/api-keys\n- name: MCP OAuth 2.1\n  type: oauth2\n  description: The MCP server (https://mcp.us-1.kognitos.com/) supports OAuth 2.1 for interactive clients\n    (Claude Desktop, Claude Code, Claude.ai) - browser login and approval, short-lived tokens refreshed by\n    the client, access scoped to the user's account and permissions. Documented as recommended over API\n    keys for interactive clients. No scope list is published.\n  applies_to: Kognitos MCP Server only\n  sources:\n  - https://docs.kognitos.com/guides/mcp/mcp\npermission_levels:\n- name: All\n  access: Full read and write access to all API endpoints, including run archiving\n- name: Read only\n  access: Read access only (list, get, query endpoints)\n- name: Restricted\n  access: Custom per-resource permissions (includes granular control over run management and archiving)\nlegacy:\n  note: The legacy REST API v1/v2 (rest-api.app.kognitos.com) authenticates with an x-api-key\
  \ header.\n  source: https://docs.kognitos.com/legacy/legacy-experience/rest-api/migrating-to-v2\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kognitos/refs/heads/main/authentication/kognitos-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Agentic AI
- Automation
- Workflow Automation
- Finance Automation
- Accounts Payable
- Neurosymbolic AI
- Enterprise
---
