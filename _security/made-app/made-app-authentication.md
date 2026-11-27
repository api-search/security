---
anonymous_access: false
api_key_in: []
api_specs:
- filename: made-app-account-api-openapi.yml
  format: yaml
  label: Made Account API
  slug: made-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/made-app/openapi/made-app-account-api-openapi.yml
- filename: made-app-batches-api-openapi.yml
  format: yaml
  label: Made Batches API
  slug: made-app-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/made-app/openapi/made-app-batches-api-openapi.yml
- filename: made-app-editing-api-openapi.yml
  format: yaml
  label: Made Editing API
  slug: made-app-editing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/made-app/openapi/made-app-editing-api-openapi.yml
- filename: made-app-generations-api-openapi.yml
  format: yaml
  label: Made Generations API
  slug: made-app-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/made-app/openapi/made-app-generations-api-openapi.yml
- filename: made-app-media-api-openapi.yml
  format: yaml
  label: Made Media API
  slug: made-app-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/made-app/openapi/made-app-media-api-openapi.yml
- filename: made-app-meta-api-openapi.yml
  format: yaml
  label: Made Meta API
  slug: made-app-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/made-app/openapi/made-app-meta-api-openapi.yml
- filename: made-app-models-api-openapi.yml
  format: yaml
  label: Made Models API
  slug: made-app-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/made-app/openapi/made-app-models-api-openapi.yml
- filename: made-app-openai-compatible-api-openapi.yml
  format: yaml
  label: Made Open AI Compatible API
  slug: made-app-openai-compatible-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/made-app/openapi/made-app-openai-compatible-api-openapi.yml
- filename: made-app-tools-api-openapi.yml
  format: yaml
  label: Made Tools API
  slug: made-app-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/made-app/openapi/made-app-tools-api-openapi.yml
auth_types: []
description: Made API uses a secret API key that must be sent as a bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Made Authentication
name_suffix: Authentication
oauth_flows: []
overview: Made declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Made
provider_slug: made-app
scheme_count: 1
schemes:
- evidence: Send it as a bearer token from your server, never from a browser.
  header: Authorization
  how_to_obtain: Create a key in Account → API keys; its secret is shown once.
  location: header
  name: Bearer
  type: http-bearer
slug: made-app-authentication
source_filename: made-app-authentication.yml
source_heading: Authentication Profile
source_url: https://www.made.app/developers
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.made.app/developers\nsources:\n- https://www.made.app/developers\ndescription: Made API uses a secret API key that must be sent as a bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Send it as a bearer token from your server, never from a browser.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Account → API keys; its secret is shown once.\nnote: No other authentication methods (apiKey, oauth2, etc.) are documented on the page.\ndocs: https://www.made.app/developers\n"
source_yaml_url: https://artifacts.apis.io/made-app/authentication/made-app-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Image Generation
- Video Generation
- Creative Tools
- Platform
---
