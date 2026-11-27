---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lemmebuyit-com-changes-api-openapi.yml
  format: yaml
  label: LemMeBuyIt Changes API
  slug: lemmebuyit-com-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lemmebuyit-com/openapi/lemmebuyit-com-changes-api-openapi.yml
- filename: lemmebuyit-com-promotions-api-openapi.yml
  format: yaml
  label: LemMeBuyIt Promotions API
  slug: lemmebuyit-com-promotions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lemmebuyit-com/openapi/lemmebuyit-com-promotions-api-openapi.yml
- filename: lemmebuyit-com-retailers-api-openapi.yml
  format: yaml
  label: LemMeBuyIt Retailers API
  slug: lemmebuyit-com-retailers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lemmebuyit-com/openapi/lemmebuyit-com-retailers-api-openapi.yml
- filename: lemmebuyit-com-status-api-openapi.yml
  format: yaml
  label: LemMeBuyIt Status API
  slug: lemmebuyit-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lemmebuyit-com/openapi/lemmebuyit-com-status-api-openapi.yml
auth_types: []
description: Authentication methods for LemMeBuyIt MCP endpoint
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LemMeBuyIt Authentication
name_suffix: Authentication
oauth_flows: []
overview: LemMeBuyIt declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LemMeBuyIt
provider_slug: lemmebuyit-com
scheme_count: 2
schemes:
- evidence: OAuth signs you in.
  name: OAuth
  type: oauth2
- evidence: 'send the header `X-API-Key: lbi_…` (create a key at https://lemmebuyit.com/dashboard/api-keys).'
  header: X-API-Key
  how_to_obtain: Create a key at https://lemmebuyit.com/dashboard/api-keys
  location: header
  name: API Key
  type: apiKey
slug: lemmebuyit-com-authentication
source_filename: lemmebuyit-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.lemmebuyit.com/docs.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.lemmebuyit.com/docs.md\nsources:\n- https://www.lemmebuyit.com/docs.md\n- https://www.lemmebuyit.com/docs\ndescription: Authentication methods for LemMeBuyIt MCP endpoint\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: OAuth signs you in.\n- type: apiKey\n  name: API Key\n  evidence: 'send the header `X-API-Key: lbi_…` (create a key at https://lemmebuyit.com/dashboard/api-keys).'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a key at https://lemmebuyit.com/dashboard/api-keys\ndocs: https://www.lemmebuyit.com/docs.md\n"
source_yaml_url: https://artifacts.apis.io/lemmebuyit-com/authentication/lemmebuyit-com-authentication.yml
summary_line: 2 schemes
tags:
- Retail
- Real-Time Data
- Product Intelligence
- AI Agents
---
