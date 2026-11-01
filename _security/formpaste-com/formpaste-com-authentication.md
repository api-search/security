---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Formpaste uses two authentication mechanisms: an API token (Bearer) for the MCP server and an access key for form submissions.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Formpaste Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: formpaste-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: formpaste-com
provider_slug: formpaste-com
scheme_count: 2
schemes:
- evidence: An account API token ( fpat_… ) is the Bearer credential that authorizes requests to the MCP server at POST /mcp .
  header: Authorization
  how_to_obtain: Mint a token in the dashboard → Settings → API & MCP and copy the raw token shown once.
  location: header
  name: API token
  type: http-bearer
- evidence: Every form gets its own access key ( fp_… ), shown on the form’s Setup tab. This is what authorizes a submission - treat it like a form ID, not a secret; it’s meant to sit in a public HTML page.
  how_to_obtain: Create a form in the dashboard; the access key is displayed on the form’s Setup tab.
  location: body
  name: access_key
  type: apiKey
slug: formpaste-com-authentication
source_filename: formpaste-com-authentication.yml
source_heading: Authentication Profile
source_url: https://formpaste.com/docs/agents/api-tokens
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://formpaste.com/docs/agents/api-tokens\nsources:\n- https://formpaste.com/docs/agents/api-tokens\n- https://formpaste.com/docs/quickstart\n- https://formpaste.com/docs/guides/ai-agent-setup\ndescription: 'Formpaste uses two authentication mechanisms: an API token (Bearer) for the MCP server and an access key for form submissions.'\nschemes:\n- type: http-bearer\n  name: API token\n  evidence: An account API token ( fpat_… ) is the Bearer credential that authorizes requests to the MCP server at POST /mcp .\n  location: header\n  header: Authorization\n  how_to_obtain: Mint a token in the dashboard → Settings → API & MCP and copy the raw token shown once.\n- type: apiKey\n  name: access_key\n  evidence: Every form gets its own access key ( fp_… ), shown on the form’s Setup tab. This is what authorizes a submission - treat it like a\n    form ID, not a secret; it’s meant to sit\
  \ in a public HTML page.\n  location: body\n  how_to_obtain: Create a form in the dashboard; the access key is displayed on the form’s Setup tab.\nnote: No OAuth2 flows, JWT, HMAC, MTLS, or other schemes are documented.\ndocs: https://formpaste.com/docs/agents/api-tokens\n"
source_yaml_url: https://artifacts.apis.io/formpaste-com/authentication/formpaste-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API
- Form
- Contact
- Free
---
