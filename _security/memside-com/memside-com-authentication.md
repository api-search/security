---
anonymous_access: false
api_key_in: []
api_specs:
- filename: memside-com-context-api-openapi.yml
  format: yaml
  label: Memside Context API
  slug: memside-com-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memside-com/openapi/memside-com-context-api-openapi.yml
- filename: memside-com-library-api-openapi.yml
  format: yaml
  label: Memside Library API
  slug: memside-com-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memside-com/openapi/memside-com-library-api-openapi.yml
- filename: memside-com-memories-api-openapi.yml
  format: yaml
  label: Memside Memories API
  slug: memside-com-memories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memside-com/openapi/memside-com-memories-api-openapi.yml
- filename: memside-com-subjects-api-openapi.yml
  format: yaml
  label: Memside Subjects API
  slug: memside-com-subjects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memside-com/openapi/memside-com-subjects-api-openapi.yml
auth_types: []
description: Memside authenticates API requests using an API key sent as a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Memside Authentication
name_suffix: Authentication
oauth_flows: []
overview: Memside declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Memside
provider_slug: memside-com
scheme_count: 1
schemes:
- evidence: 'Send the key as a bearer token: Authorization: Bearer mem_sk_example_key'
  header: Authorization
  how_to_obtain: Create a key in Settings > Developer & API, copy it immediately, and store it (e.g., in an environment variable).
  location: header
  name: API Key
  type: http-bearer
slug: memside-com-authentication
source_filename: memside-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.memside.com/developers/api-keys/
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.memside.com/developers/api-keys/\nsources:\n- https://docs.memside.com/developers/api-keys/\n- https://docs.memside.com/developers/api-keys/\n- https://docs.memside.com/getting-started/\n- https://docs.memside.com/developers/\ndescription: Memside authenticates API requests using an API key sent as a Bearer token.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Send the key as a bearer token: Authorization: Bearer mem_sk_example_key'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Settings > Developer & API, copy it immediately, and store it (e.g., in an environment variable).\nnote: No OAuth2, apiKey, http-basic, jwt, hmac, mtls, or other authentication schemes are documented.\ndocs: https://docs.memside.com/developers/api-keys/\n"
source_yaml_url: https://artifacts.apis.io/memside-com/authentication/memside-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Memory
- Continuity
- Platform
- Company
---
