---
anonymous_access: false
api_key_in: []
api_specs:
- filename: curviate-com-openapi.json
  format: json
  label: Curviate API
  slug: curviate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curviate-com/openapi/curviate-com-openapi.json
auth_types: []
description: Curviate supports OAuth 2.1, a Bearer header, and a token query parameter for authentication.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Curviate Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: curviate-com declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: curviate-com
provider_slug: curviate-com
scheme_count: 3
schemes:
- evidence: Use OAuth wherever the client supports it, a header where it does not, and the query parameter only when the client can set no header at all.
  how_to_obtain: Sign in to Curviate in the browser and approve the client on a consent screen; the client receives its own tokens.
  name: OAuth 2.1
  type: oauth2
- evidence: 'Bearer header Send Authorization: Bearer cvt_live_YOUR_KEY on every request.'
  header: Authorization
  how_to_obtain: Copy the API key from the key chip in the dashboard top bar and use it as the Bearer token.
  location: header
  name: Bearer header
  type: http-bearer
- evidence: ?token= https://app.curviate.com/mcp?token=cvt_live_YOUR_KEY The client can set neither OAuth nor a header.
  how_to_obtain: Copy the API key from the dashboard and append it as the token query parameter.
  location: query
  name: Token query parameter
  type: apiKey
slug: curviate-com-authentication
source_filename: curviate-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.curviate.com/reference/mcp/quickstart
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.curviate.com/reference/mcp/quickstart\nsources:\n- https://docs.curviate.com/reference/mcp/quickstart\n- https://docs.curviate.com/reference/mcp/client-setup\n- https://docs.curviate.com/reference/cli/setup-and-doctor\ndescription: Curviate supports OAuth 2.1, a Bearer header, and a token query parameter for authentication.\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Use OAuth wherever the client supports it, a header where it does not, and the query parameter only when the client can set no header\n    at all.\n  how_to_obtain: Sign in to Curviate in the browser and approve the client on a consent screen; the client receives its own tokens.\n- type: http-bearer\n  name: Bearer header\n  evidence: 'Bearer header Send Authorization: Bearer cvt_live_YOUR_KEY on every request.'\n  location: header\n  header: Authorization\n  how_to_obtain: Copy the API key\
  \ from the key chip in the dashboard top bar and use it as the Bearer token.\n- type: apiKey\n  name: Token query parameter\n  evidence: ?token= https://app.curviate.com/mcp?token=cvt_live_YOUR_KEY The client can set neither OAuth nor a header.\n  location: query\n  how_to_obtain: Copy the API key from the dashboard and append it as the token query parameter.\ndocs: https://docs.curviate.com/reference/mcp/quickstart\n"
source_yaml_url: https://artifacts.apis.io/curviate-com/authentication/curviate-com-authentication.yml
summary_line: 3 schemes
tags:
- AI
- LinkedIn
- API
- Automation
- Agent
---
