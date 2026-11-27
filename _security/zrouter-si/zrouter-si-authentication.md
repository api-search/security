---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: zrouter-si Authentication
name_suffix: Authentication
oauth_flows: []
overview: zrouter-si declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: zrouter-si
provider_slug: zrouter-si
scheme_count: 1
schemes:
- evidence: 'Authentication Create an account API key in your dashboard and include it in every inference request: Authorization: Bearer YOUR_ZROUTER_KEY'
  header: Authorization
  how_to_obtain: Create an account API key in your dashboard.
  location: header
  name: Authorization
  type: http-bearer
slug: zrouter-si-authentication
source_filename: zrouter-si-authentication.yml
source_heading: Authentication Profile
source_url: https://zrouter.si/docs/api
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://zrouter.si/docs/api\nsources:\n- https://zrouter.si/docs/api\n- https://zrouter.si/docs/integrations/claude-code\n- https://zrouter.si/docs/byok\n- https://zrouter.si/docs/credits\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Authentication Create an account API key in your dashboard and include it in every inference request: Authorization: Bearer YOUR_ZROUTER_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an account API key in your dashboard.\ndocs: https://zrouter.si/docs/api\n"
source_yaml_url: https://artifacts.apis.io/zrouter-si/authentication/zrouter-si-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- API Gateway
- OpenAI-Compatible
- Multi-Model
---
