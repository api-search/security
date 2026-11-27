---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for openaso
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: openaso Authentication
name_suffix: Authentication
oauth_flows: []
overview: openaso declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: openaso
provider_slug: openaso-ai
scheme_count: 2
schemes:
- evidence: '--header "Authorization: Bearer YOUR_KEY"'
  header: Authorization
  how_to_obtain: Create an account at https://openaso.ai/login, then mint an API key in the dashboard at https://openaso.ai/dashboard.
  location: header
  name: Bearer
  type: http-bearer
- evidence: 'x-api-key: YOUR_KEY works too if your client cannot set an Authorization header.'
  header: x-api-key
  how_to_obtain: Create an account at https://openaso.ai/login, then mint an API key in the dashboard at https://openaso.ai/dashboard.
  location: header
  name: apiKey
  type: apiKey
slug: openaso-ai-authentication
source_filename: openaso-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://openaso.ai/docs.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://openaso.ai/docs.md\nsources:\n- https://openaso.ai/docs.md\n- https://openaso.ai/docs\ndescription: Authentication schemes for openaso\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '--header \"Authorization: Bearer YOUR_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an account at https://openaso.ai/login, then mint an API key in the dashboard at https://openaso.ai/dashboard.\n- type: apiKey\n  name: apiKey\n  evidence: 'x-api-key: YOUR_KEY works too if your client cannot set an Authorization header.'\n  location: header\n  header: x-api-key\n  how_to_obtain: Create an account at https://openaso.ai/login, then mint an API key in the dashboard at https://openaso.ai/dashboard.\ndocs: https://openaso.ai/docs.md\n"
source_yaml_url: https://artifacts.apis.io/openaso-ai/authentication/openaso-ai-authentication.yml
summary_line: 2 schemes
tags:
- ASO
- MCP
- Artificial Intelligence
- App Store
- Optimization
---
