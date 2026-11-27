---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mentiondrop-com-openapi-generated.yml
  format: yaml
  label: MentionDrop API
  slug: mentiondrop-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentiondrop-com/openapi/_ae-authored/mentiondrop-com-openapi-generated.yml
auth_types: []
description: MentionDrop uses API‑key authentication where the key is sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MentionDrop Authentication
name_suffix: Authentication
oauth_flows: []
overview: MentionDrop declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MentionDrop
provider_slug: mentiondrop-com
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer md_live_xxx'
  header: Authorization
  how_to_obtain: Create an API key in Settings; keys are prefixed md_live_.
  location: header
  name: API key
  type: http-bearer
slug: mentiondrop-com-authentication
source_filename: mentiondrop-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.mentiondrop.com/docs/mcp
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.mentiondrop.com/docs/mcp\nsources:\n- https://www.mentiondrop.com/docs/mcp\ndescription: MentionDrop uses API‑key authentication where the key is sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Authorization: Bearer md_live_xxx'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings; keys are prefixed md_live_.\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the page.\ndocs: https://www.mentiondrop.com/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/mentiondrop-com/authentication/mentiondrop-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Brand Monitoring
- Artificial Intelligence
- Software-as-a-Service
- Marketing
---
