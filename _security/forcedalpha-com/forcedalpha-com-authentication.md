---
anonymous_access: false
api_key_in: []
api_specs:
- filename: forcedalpha-com-openapi-generated.yml
  format: yaml
  label: Forced Alpha API
  slug: forcedalpha-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forcedalpha-com/openapi/_ae-authored/forcedalpha-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Forced Alpha MCP API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Forced Alpha Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forced Alpha declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Forced Alpha
provider_slug: forcedalpha-com
scheme_count: 2
schemes:
- evidence: For live MCP use, account authorization is required through OAuth or an account‑issued API key for `https://forcedalpha.com/mcp/`.
  how_to_obtain: 'Credentials are issued after email verification; see the account and key flow documentation linked in the page.

    https://forcedalpha.com/docs/mcp/#get-key-detail (link provided in text).'
  name: API Key
  type: apiKey
- evidence: For live MCP use, account authorization is required through OAuth or an account‑issued API key for `https://forcedalpha.com/mcp/`.
  how_to_obtain: OAuth flow is described in the account and key flow documentation; the page does not provide token or authorize URLs, flow types, or scopes.
  name: OAuth
  type: oauth2
slug: forcedalpha-com-authentication
source_filename: forcedalpha-com-authentication.yml
source_heading: Authentication Profile
source_url: https://forcedalpha.com/tools/casefiles/token-value-compounding/
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://forcedalpha.com/tools/casefiles/token-value-compounding/\nsources:\n- https://forcedalpha.com/tools/casefiles/token-value-compounding/\n- https://forcedalpha.com/agents/quickstart.md\ndescription: Authentication methods for Forced Alpha MCP API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: For live MCP use, account authorization is required through OAuth or an account‑issued API key for `https://forcedalpha.com/mcp/`.\n  how_to_obtain: 'Credentials are issued after email verification; see the account and key flow documentation linked in the page.\n\n    https://forcedalpha.com/docs/mcp/#get-key-detail (link provided in text).'\n- type: oauth2\n  name: OAuth\n  evidence: For live MCP use, account authorization is required through OAuth or an account‑issued API key for `https://forcedalpha.com/mcp/`.\n  how_to_obtain: OAuth flow is described in the account and key\
  \ flow documentation; the page does not provide token or authorize URLs, flow types,\n    or scopes.\ndocs: https://forcedalpha.com/tools/casefiles/token-value-compounding/\n"
source_yaml_url: https://artifacts.apis.io/forcedalpha-com/authentication/forcedalpha-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Supply Chain
- Investment
- Data Intelligence
- Portfolio
---
