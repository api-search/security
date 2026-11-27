---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: contractors.fyi Authentication
name_suffix: Authentication
oauth_flows: []
overview: contractors.fyi declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: contractors.fyi
provider_slug: contractors-fyi
scheme_count: 1
schemes:
- applies_to:
  - https://contractors.fyi/mcp
  - https://contractors.fyi/*.json
  description: The MCP server and the per-city JSON data files are public and keyless.
  evidence:
  - quote: No account and no key. It only reads public data.
    url: https://contractors.fyi/ai/
  - quote: Create an app with the address https://contractors.fyi/mcp and no authentication.
    url: https://contractors.fyi/ai/
  - quote: the same data as tools for AI assistants (ranked contractors, permit costs and timelines, solar and generator sizing); no key needed
    url: https://contractors.fyi/llms.txt
  type: none
slug: contractors-fyi-authentication
source_filename: contractors-fyi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://contractors.fyi/ai/\ndocs: https://contractors.fyi/ai/\nname: contractors.fyi authentication\nschemes:\n- type: none\n  applies_to:\n  - https://contractors.fyi/mcp\n  - https://contractors.fyi/*.json\n  description: The MCP server and the per-city JSON data files are public and keyless.\n  evidence:\n  - quote: No account and no key. It only reads public data.\n    url: https://contractors.fyi/ai/\n  - quote: Create an app with the address https://contractors.fyi/mcp and no authentication.\n    url: https://contractors.fyi/ai/\n  - quote: 'the same data as tools for AI assistants (ranked contractors, permit costs and timelines, solar and generator sizing); no key needed'\n    url: https://contractors.fyi/llms.txt\nnote: A consumer \"Sign in\" page (https://contractors.fyi/signin/) exists for the website account; it is not documented as an API credential and was not called.\n"
source_yaml_url: https://artifacts.apis.io/contractors-fyi/authentication/contractors-fyi-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Contractors
- Home Improvement
- Building Permits
- Public Records
- MCP
- Real Estate
---
