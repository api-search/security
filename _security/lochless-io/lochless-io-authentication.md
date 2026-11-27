---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lochless-io-ask-api-openapi.yml
  format: yaml
  label: Lochless Ask API
  slug: lochless-io-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lochless-io/openapi/lochless-io-ask-api-openapi.yml
- filename: lochless-io-context-api-openapi.yml
  format: yaml
  label: Lochless Context API
  slug: lochless-io-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lochless-io/openapi/lochless-io-context-api-openapi.yml
- filename: lochless-io-dashboards-api-openapi.yml
  format: yaml
  label: Lochless Dashboards API
  slug: lochless-io-dashboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lochless-io/openapi/lochless-io-dashboards-api-openapi.yml
- filename: lochless-io-docs-api-openapi.yml
  format: yaml
  label: Lochless Docs API
  slug: lochless-io-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lochless-io/openapi/lochless-io-docs-api-openapi.yml
- filename: lochless-io-ingest-api-openapi.yml
  format: yaml
  label: Lochless Ingest API
  slug: lochless-io-ingest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lochless-io/openapi/lochless-io-ingest-api-openapi.yml
- filename: lochless-io-recorder-api-openapi.yml
  format: yaml
  label: Lochless Recorder API
  slug: lochless-io-recorder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lochless-io/openapi/lochless-io-recorder-api-openapi.yml
- filename: lochless-io-widgets-api-openapi.yml
  format: yaml
  label: Lochless Widgets API
  slug: lochless-io-widgets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lochless-io/openapi/lochless-io-widgets-api-openapi.yml
auth_types: []
description: Every request uses the same key as a bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lochless Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lochless declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lochless
provider_slug: lochless-io
scheme_count: 1
schemes:
- evidence: Every request uses the same key as a bearer token.
  header: Authorization
  how_to_obtain: Sign in with Google at console.lochless.io, request access, then create an API key in the console.
  location: header
  name: API Key
  type: http-bearer
slug: lochless-io-authentication
source_filename: lochless-io-authentication.yml
source_heading: Authentication Profile
source_url: https://lochless.io/docs.html
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lochless.io/docs.html\nsources:\n- https://lochless.io/docs.html\ndescription: Every request uses the same key as a bearer token.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Every request uses the same key as a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in with Google at console.lochless.io, request access, then create an API key in the console.\nnote: No OAuth2 flows, API key rotation, or other authentication schemes are documented on the page.\ndocs: https://lochless.io/docs.html\n"
source_yaml_url: https://artifacts.apis.io/lochless-io/authentication/lochless-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- RAG
- Artificial Intelligence
- Search
- Documentation
---
