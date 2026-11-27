---
anonymous_access: false
api_key_in: []
api_specs:
- filename: completionkit-com-openapi-generated.yml
  format: yaml
  label: CompletionKit API
  slug: completionkit-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/completionkit-com/openapi/_ae-authored/completionkit-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CompletionKit Authentication
name_suffix: Authentication
oauth_flows: []
overview: CompletionKit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CompletionKit
provider_slug: completionkit-com
scheme_count: 1
schemes:
- applies_to:
  - REST API /orgs/{org-slug}/api/v1
  - MCP server /orgs/{org-slug}/mcp
  description: 'Authenticate with a bearer key in the Authorization header: create one under Settings → API once you''ve made an organization.'
  header: Authorization
  in: header
  name: bearer
  scheme: bearer
  scoping: per organization (the org slug is part of every path)
  type: http
slug: completionkit-com-authentication
source_filename: completionkit-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://completionkit.com/docs/api\ndocs: https://completionkit.com/docs/api\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: \"Authenticate with a bearer key in the Authorization header: create one under Settings → API once you've made an organization.\"\n  applies_to: ['REST API /orgs/{org-slug}/api/v1', 'MCP server /orgs/{org-slug}/mcp']\n  scoping: per organization (the org slug is part of every path)\noauth: false\nnote: No OAuth flows or permission scopes are documented; keys are organization-scoped bearer tokens.\n"
source_yaml_url: https://artifacts.apis.io/completionkit-com/authentication/completionkit-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- LLM
- Prompt Engineering
- Evaluation
- Testing
- Developer Tools
- MCP
---
