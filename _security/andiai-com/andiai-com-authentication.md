---
anonymous_access: false
api_key_in: []
api_specs:
- filename: andiai-com-search-api-openapi.yml
  format: yaml
  label: Andi AI Search API
  slug: andiai-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andiai-com/openapi/andiai-com-search-api-openapi.yml
auth_types: []
description: Authentication schemes for Andi AI
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Andi AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Andi AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Andi AI
provider_slug: andiai-com
scheme_count: 1
schemes:
- evidence: Authenticate with the Andi AI Search API using API keys in the x-api-key header.
  header: x-api-key
  how_to_obtain: Create a key in the API Console (https://console.andiai.com) and copy it.
  location: header
  name: API Key
  type: apiKey
slug: andiai-com-authentication
source_filename: andiai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.andiai.com/getting-started/authentication.md
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.andiai.com/getting-started/authentication.md\nsources:\n- https://docs.andiai.com/getting-started/authentication.md\n- https://docs.andiai.com/getting-started/quickstart.md\n- https://docs.andiai.com/getting-started/cli.md\ndescription: Authentication schemes for Andi AI\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Authenticate with the Andi AI Search API using API keys in the x-api-key header.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a key in the API Console (https://console.andiai.com) and copy it.\nnote: No OAuth2, HTTP Bearer, or other authentication methods are documented.\ndocs: https://docs.andiai.com/getting-started/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/andiai-com/authentication/andiai-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Search
- Privacy
- OpenAI
- Community
---
