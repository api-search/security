---
anonymous_access: false
api_key_in: []
api_specs:
- filename: applyra-io-openapi-generated.yml
  format: yaml
  label: Applyra API
  slug: applyra-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/applyra-io/openapi/_ae-authored/applyra-io-openapi-generated.yml
auth_types: []
description: Applyra API authentication uses an API key.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Applyra Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Applyra declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Applyra
provider_slug: applyra-io
scheme_count: 2
schemes:
- evidence: Every Applyra API request carries a personal key, in an X-API-Key header or an api_key query parameter.
  header: X-API-Key
  location: header
  name: X-API-Key
  type: apiKey
- evidence: Every Applyra API request carries a personal key, in an X-API-Key header or an api_key query parameter.
  location: query
  name: api_key
  type: apiKey
slug: applyra-io-authentication
source_filename: applyra-io-authentication.yml
source_heading: Authentication Profile
source_url: https://www.applyra.io/docs/api/errors-and-limits
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.applyra.io/docs/api/errors-and-limits\nsources:\n- https://www.applyra.io/docs/api/errors-and-limits\n- https://www.applyra.io/docs/getting-started/what-is-applyra\n- https://www.applyra.io/docs/getting-started/add-your-first-app\n- https://www.applyra.io/docs/getting-started/add-your-first-keywords\ndescription: Applyra API authentication uses an API key.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Every Applyra API request carries a personal key, in an X-API-Key header or an api_key query parameter.\n  location: header\n  header: X-API-Key\n- type: apiKey\n  name: api_key\n  evidence: Every Applyra API request carries a personal key, in an X-API-Key header or an api_key query parameter.\n  location: query\ndocs: https://www.applyra.io/docs/api/errors-and-limits\n"
source_yaml_url: https://artifacts.apis.io/applyra-io/authentication/applyra-io-authentication.yml
summary_line: 2 schemes
tags:
- ASO
- Mobile
- Analytics
- Artificial Intelligence
- Indie
---
