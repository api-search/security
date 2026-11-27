---
anonymous_access: false
api_key_in: []
api_specs:
- filename: financialfilings-com-openapi.yml
  format: yaml
  label: Financial Filings API
  slug: financial-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/financialfilings-com/openapi/financialfilings-com-openapi.yml
auth_types: []
description: Authentication is performed via OAuth 2.0 using a free FinancialFilings account. The flow occurs in the browser where the user signs in; no API key is required.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FinancialFilings Authentication
name_suffix: Authentication
oauth_flows: []
overview: FinancialFilings declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FinancialFilings
provider_slug: financialfilings-com
scheme_count: 1
schemes:
- evidence: Auth OAuth 2.0 · free account
  how_to_obtain: Sign in with a free FinancialFilings account via the browser (OAuth flow).
  name: OAuth 2.0
  type: oauth2
slug: financialfilings-com-authentication
source_filename: financialfilings-com-authentication.yml
source_heading: Authentication Profile
source_url: https://financialfilings.com/mcp/
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://financialfilings.com/mcp/\nsources:\n- https://financialfilings.com/mcp/\n- https://financialfilings.com/integrations/claude/\n- https://financialfilings.com/integrations/claude-code/\n- https://financialfilings.com/integrations/chatgpt/\ndescription: Authentication is performed via OAuth 2.0 using a free FinancialFilings account. The flow occurs in the browser where the user signs\n  in; no API key is required.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: Auth OAuth 2.0 · free account\n  how_to_obtain: Sign in with a free FinancialFilings account via the browser (OAuth flow).\ndocs: https://financialfilings.com/mcp/\n"
source_yaml_url: https://artifacts.apis.io/financialfilings-com/authentication/financialfilings-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Financial Data
- Filings
- Market Data
- Research
---
