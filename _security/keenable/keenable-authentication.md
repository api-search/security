---
anonymous_access: false
api_key_in: []
api_specs:
- filename: keenable-fetch-api-openapi.yml
  format: yaml
  label: Keenable Fetch API
  slug: keenable-fetch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keenable/openapi/keenable-fetch-api-openapi.yml
- filename: keenable-search-api-openapi.yml
  format: yaml
  label: Keenable Search API
  slug: keenable-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keenable/openapi/keenable-search-api-openapi.yml
auth_types: []
description: Keenable authenticates with an API key. Obtain a key by logging in to the console.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Keenable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keenable declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Keenable
provider_slug: keenable
scheme_count: 2
schemes:
- evidence: Keenable authenticates with an API key. [Log in](https://app.keenable.ai/login) to obtain one.
  header: X-API-Key
  how_to_obtain: Log in at https://app.keenable.ai/login and create an API key in the console.
  location: header
  name: API Key Header
  type: apiKey
- evidence: Alternatively, you can pass your API key in the `Authorization` header using the `Bearer` scheme.
  header: Authorization
  how_to_obtain: Log in at https://app.keenable.ai/login and create an API key in the console.
  location: header
  name: API Key Bearer
  type: http-bearer
slug: keenable-authentication
source_filename: keenable-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.keenable.ai/authentication.md
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.keenable.ai/authentication.md\nsources:\n- https://docs.keenable.ai/authentication.md\n- https://docs.keenable.ai/index.md\ndescription: Keenable authenticates with an API key. Obtain a key by logging in to the console.\nschemes:\n- type: apiKey\n  name: API Key Header\n  evidence: Keenable authenticates with an API key. [Log in](https://app.keenable.ai/login) to obtain one.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Log in at https://app.keenable.ai/login and create an API key in the console.\n- type: http-bearer\n  name: API Key Bearer\n  evidence: Alternatively, you can pass your API key in the `Authorization` header using the `Bearer` scheme.\n  location: header\n  header: Authorization\n  how_to_obtain: Log in at https://app.keenable.ai/login and create an API key in the console.\nnote: If both headers are present, `X-API-Key` takes precedence.\n\
  docs: https://docs.keenable.ai/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/keenable/authentication/keenable-authentication.yml
summary_line: 2 schemes
tags:
- Web Search
- API
- AI Agents
- AI Labs
- Inference Platforms
---
