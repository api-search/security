---
anonymous_access: false
api_key_in: []
api_specs:
- filename: consensus-app-openapi-generated.yml
  format: yaml
  label: Consensus API
  slug: consensus-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/consensus-app/openapi/_ae-authored/consensus-app-openapi-generated.yml
auth_types: []
description: Authentication methods for Consensus API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Consensus App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Consensus declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Consensus
provider_slug: consensus-app
scheme_count: 2
schemes:
- evidence: 'curl -G "https://api.consensus.app/v1/search" -H "x-api-key: $CONSENSUS_API_KEY" \'
  header: x-api-key
  location: header
  name: API Key
  type: apiKey
- evidence: API key as a Bearer token
  header: Authorization
  location: header
  name: Bearer Token
  type: http-bearer
slug: consensus-app-authentication
source_filename: consensus-app-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.consensus.app/api-quickstart-search.md
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.consensus.app/api-quickstart-search.md\nsources:\n- https://docs.consensus.app/api-quickstart-search.md\n- https://docs.consensus.app/api-quickstart-threads.md\n- https://docs.consensus.app/mcp-tools/quickstart.md\n- https://help.consensus.app/en/collections/4034444-getting-started-faqs\ndescription: Authentication methods for Consensus API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'curl -G \"https://api.consensus.app/v1/search\" -H \"x-api-key: $CONSENSUS_API_KEY\" \\'\n  location: header\n  header: x-api-key\n- type: http-bearer\n  name: Bearer Token\n  evidence: API key as a Bearer token\n  location: header\n  header: Authorization\nnote: No OAuth2 flows or other authentication schemes are documented on the provided pages.\ndocs: https://docs.consensus.app/api-quickstart-search.md\n"
source_yaml_url: https://artifacts.apis.io/consensus-app/authentication/consensus-app-authentication.yml
summary_line: 2 schemes
tags:
- AI
- EducationalApplication
---
