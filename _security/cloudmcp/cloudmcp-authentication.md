---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cloudmcp-openapi-generated.yml
  format: yaml
  label: Cloud MCP API
  slug: cloudmcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudmcp/refs/heads/main/openapi/_ae-authored/cloudmcp-openapi-generated.yml
auth_types: []
description: Authentication schemes for Cloud MCP
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cloudmcp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloud MCP declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cloud MCP
provider_slug: cloudmcp
scheme_count: 1
schemes:
- evidence: All API endpoints are authenticated using Bearer tokens and picked up from the specification file.
  header: Authorization
  location: header
  name: bearerAuth
  type: http-bearer
slug: cloudmcp-authentication
source_filename: cloudmcp-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.cloudmcp.run/api-reference/introduction#authentication
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.cloudmcp.run/api-reference/introduction#authentication\nsources:\n- https://docs.cloudmcp.run/api-reference/introduction#authentication\n- https://docs.cloudmcp.run/quickstart.md\n- https://docs.cloudmcp.run/ai-tools/cursor.md\n- https://docs.cloudmcp.run/ai-tools/claude-code.md\ndescription: Authentication schemes for Cloud MCP\nschemes:\n- type: http-bearer\n  name: bearerAuth\n  evidence: All API endpoints are authenticated using Bearer tokens and picked up from the specification file.\n  location: header\n  header: Authorization\ndocs: https://docs.cloudmcp.run/api-reference/introduction#authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudmcp/refs/heads/main/authentication/cloudmcp-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Integration
- Tools
- Automation
---
