---
anonymous_access: false
api_key_in: []
api_specs:
- filename: enhancedint-com-agent-api-openapi.yml
  format: yaml
  label: enhancedint-com Agent API
  slug: enhancedint-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enhancedint-com/openapi/enhancedint-com-agent-api-openapi.yml
- filename: enhancedint-com-mcp-api-openapi.yml
  format: yaml
  label: enhancedint-com MCP API
  slug: enhancedint-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enhancedint-com/openapi/enhancedint-com-mcp-api-openapi.yml
auth_types: []
description: Authentication is performed by checking for an auth token stored in a cookie named "auth-token".
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Enhancedint Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: enhancedint-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: enhancedint-com
provider_slug: enhancedint-com
scheme_count: 1
schemes:
- evidence: const token = request.cookies.get('auth-token');
  location: cookie
  name: auth-token
  type: apiKey
slug: enhancedint-com-authentication
source_filename: enhancedint-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.enhancedint.com/blog/getting-started-with-nextjs
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.enhancedint.com/blog/getting-started-with-nextjs\nsources:\n- https://www.enhancedint.com/blog/getting-started-with-nextjs\ndescription: Authentication is performed by checking for an auth token stored in a cookie named \"auth-token\".\nschemes:\n- type: apiKey\n  name: auth-token\n  evidence: const token = request.cookies.get('auth-token');\n  location: cookie\ndocs: https://www.enhancedint.com/blog/getting-started-with-nextjs\n"
source_yaml_url: https://artifacts.apis.io/enhancedint-com/authentication/enhancedint-com-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Websites
- Receptionist
- Booking
- LocalBusiness
- Automation
---
