---
anonymous_access: false
api_key_in: []
api_specs:
- filename: expense-budget-tracker-com-openapi-generated.yml
  format: yaml
  label: Expense Budget Tracker API
  slug: expense-budget-tracker-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/expense-budget-tracker-com/openapi/_ae-authored/expense-budget-tracker-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Expense Budget Tracker
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Expense Budget Tracker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Expense Budget Tracker declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Expense Budget Tracker
provider_slug: expense-budget-tracker-com
scheme_count: 2
schemes:
- evidence: Start the Authorization Code flow and open the authorization URL in the user's browser. Use PKCE for every authorization request. The only supported code challenge method is S256.
  flows:
  - authorization_code
  how_to_obtain: Register dynamically as a public OAuth client (no client secret) and follow the Authorization Code flow with PKCE as described.
  name: OAuth2 Authorization Code with PKCE
  scopes:
  - expenses:read
  - expenses:write
  type: oauth2
- evidence: 'Authenticated requests use: Authorization: ApiKey <key>'
  header: Authorization
  how_to_obtain: 'Obtain a long-lived ApiKey via the agent bootstrap flow: POST email to the bootstrap URL, verify the 8‑digit code at https://auth.expense-budget-tracker.com/api/agent/verify-code, and receive the ApiKey.'
  location: header
  name: ApiKey
  type: apiKey
slug: expense-budget-tracker-com-authentication
source_filename: expense-budget-tracker-com-authentication.yml
source_heading: Authentication Profile
source_url: https://expense-budget-tracker.com/docs/mcp-connector/
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://expense-budget-tracker.com/docs/mcp-connector/\nsources:\n- https://expense-budget-tracker.com/docs/mcp-connector/\n- https://expense-budget-tracker.com/docs/architecture/\n- https://expense-budget-tracker.com/docs/getting-started/\n- https://expense-budget-tracker.com/docs/agent-setup/\ndescription: Authentication methods for Expense Budget Tracker\nschemes:\n- type: oauth2\n  name: OAuth2 Authorization Code with PKCE\n  evidence: Start the Authorization Code flow and open the authorization URL in the user's browser. Use PKCE for every authorization request.\n    The only supported code challenge method is S256.\n  flows:\n  - authorization_code\n  scopes:\n  - expenses:read\n  - expenses:write\n  how_to_obtain: Register dynamically as a public OAuth client (no client secret) and follow the Authorization Code flow with PKCE as described.\n- type: apiKey\n  name: ApiKey\n\
  \  evidence: 'Authenticated requests use: Authorization: ApiKey <key>'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Obtain a long-lived ApiKey via the agent bootstrap flow: POST email to the bootstrap URL, verify the 8‑digit code at https://auth.expense-budget-tracker.com/api/agent/verify-code,\n    and receive the ApiKey.'\ndocs: https://expense-budget-tracker.com/docs/mcp-connector/\n"
source_yaml_url: https://artifacts.apis.io/expense-budget-tracker-com/authentication/expense-budget-tracker-com-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Open Source
- Personal Finance
- Budgeting
- Multi-Currency
---
