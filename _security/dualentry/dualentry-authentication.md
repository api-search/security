---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Dualentry Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: DualEntry secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: DualEntry
provider_slug: dualentry
scheme_count: 2
schemes:
- errors:
    invalid_or_revoked_key: 403 (message "API key authentication failed")
    missing_key: 401
  in: header
  issuance: Issued by an organization administrator in the DualEntry dashboard. The key is shown once at creation and cannot be retrieved afterward; store it in a secret manager or environment variable. Separate keys are recommended for development vs production.
  name: ApiKeyAuth
  parameter_name: X-API-KEY
  sources:
  - https://docs.dualentry.com/developers/guides/authentication
  surface: Public REST API (V1 + V2)
  type: apiKey
- cli_bootstrap: dualentry auth login
  description: Browser-based OAuth 2.1 sign-in. The CLI stores credentials in the system keychain; the MCP server (https://api.dualentry.com/mcp/) signs in per client. Permissions are scoped to the authenticated user's DualEntry role. No public scope reference is documented.
  flow: authorizationCode
  headless_alternative: X_API_KEY environment variable (CI/CD)
  name: OAuth2
  scheme: OAuth 2.1
  sources:
  - https://docs.dualentry.com/developers/guides/mcp-integration
  - https://docs.dualentry.com/developers/guides/cli-quickstart
  surface: Hosted MCP server + DualEntry CLI
  type: oauth2
slug: dualentry-authentication
source_filename: dualentry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.dualentry.com/developers/guides/authentication\ndocs: https://docs.dualentry.com/developers/guides/authentication\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  api_key_header: X-API-KEY\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    The DualEntry Public REST API authenticates with a static API key in the\n    X-API-KEY header. The hosted MCP server and the first-party CLI authenticate\n    with OAuth 2.1 browser sign-in instead (no API keys), where permissions match\n    the signed-in user's DualEntry role.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: X-API-KEY\n  surface: Public REST API (V1 + V2)\n  issuance: >-\n    Issued by an organization administrator in the DualEntry dashboard. The key\n    is shown once at creation and cannot be retrieved afterward; store it in a\n    secret manager or environment variable. Separate keys are recommended for\n\
  \    development vs production.\n  errors:\n    missing_key: 401\n    invalid_or_revoked_key: 403 (message \"API key authentication failed\")\n  sources: [https://docs.dualentry.com/developers/guides/authentication]\n- name: OAuth2\n  type: oauth2\n  scheme: OAuth 2.1\n  surface: Hosted MCP server + DualEntry CLI\n  flow: authorizationCode\n  description: >-\n    Browser-based OAuth 2.1 sign-in. The CLI stores credentials in the system\n    keychain; the MCP server (https://api.dualentry.com/mcp/) signs in per\n    client. Permissions are scoped to the authenticated user's DualEntry role.\n    No public scope reference is documented.\n  cli_bootstrap: dualentry auth login\n  headless_alternative: X_API_KEY environment variable (CI/CD)\n  sources:\n  - https://docs.dualentry.com/developers/guides/mcp-integration\n  - https://docs.dualentry.com/developers/guides/cli-quickstart\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dualentry/refs/heads/main/authentication/dualentry-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- AI
- Accounting
- ERP
- Finance
- Financial Operations
- Bookkeeping
- Revenue Recognition
- Fintech
---
