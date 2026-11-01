---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mojeek-search-api-openapi.yml
  format: yaml
  label: Mojeek Search API
  slug: mojeek-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mojeek/openapi/mojeek-search-api-openapi.yml
- filename: mojeek-openapi-generated.yml
  format: yaml
  label: Mojeek API
  slug: mojeek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mojeek/openapi/_ae-authored/mojeek-openapi-generated.yml
auth_types: []
description: Authentication is performed using an API key passed as a query parameter.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mojeek Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mojeek declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mojeek
provider_slug: mojeek
scheme_count: 1
schemes:
- evidence: curl "https://api.mojeek.com/search?q=mojeek&api_key=YOUR_API_KEY&lb=EN&lbb=100&rb=GB&rbb=10&fmt=json"
  how_to_obtain: An active account and API key. Sign‑up and details can be found on the Mojeek Search API page.
  location: query
  name: api_key
  type: apiKey
slug: mojeek-authentication
source_filename: mojeek-authentication.yml
source_heading: Authentication Profile
source_url: https://www.mojeek.com/support/api/search/quickstart.html
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.mojeek.com/support/api/search/quickstart.html\nsources:\n- https://www.mojeek.com/support/api/search/quickstart.html\ndescription: Authentication is performed using an API key passed as a query parameter.\nschemes:\n- type: apiKey\n  name: api_key\n  evidence: curl \"https://api.mojeek.com/search?q=mojeek&api_key=YOUR_API_KEY&lb=EN&lbb=100&rb=GB&rbb=10&fmt=json\"\n  location: query\n  how_to_obtain: An active account and API key. Sign‑up and details can be found on the Mojeek Search API page.\ndocs: https://www.mojeek.com/support/api/search/quickstart.html\n"
source_yaml_url: https://artifacts.apis.io/mojeek/authentication/mojeek-authentication.yml
summary_line: 1 scheme
tags:
- Search
- Privacy
- API
- Open-source
- Community
---
