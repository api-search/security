---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bfocus-com-br-openapi.json
  format: json
  label: bFocus API
  slug: bfocus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bfocus-com-br/openapi/bfocus-com-br-openapi.json
auth_types: []
description: Authentication for bFocus API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bfocus Com Br Authentication
name_suffix: Authentication
oauth_flows: []
overview: bFocus declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: bFocus
provider_slug: bfocus-com-br
scheme_count: 1
schemes:
- evidence: 'Every request carries Authorization: Bearer.'
  header: Authorization
  how_to_obtain: Generate the key under Integrations › API keys in the bFocus dashboard.
  location: header
  name: API Key
  type: http-bearer
slug: bfocus-com-br-authentication
source_filename: bfocus-com-br-authentication.yml
source_heading: Authentication Profile
source_url: https://www.bfocus.com.br/en/desenvolvedores
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.bfocus.com.br/en/desenvolvedores\nsources:\n- https://www.bfocus.com.br/en/desenvolvedores\ndescription: Authentication for bFocus API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Every request carries Authorization: Bearer.'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate the key under Integrations › API keys in the bFocus dashboard.\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the page.\ndocs: https://www.bfocus.com.br/en/desenvolvedores\n"
source_yaml_url: https://artifacts.apis.io/bfocus-com-br/authentication/bfocus-com-br-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Lead Management
- Customer Service
- Software-as-a-Service
- Brazil
---
