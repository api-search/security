---
anonymous_access: false
api_key_in: []
api_specs:
- filename: feason-com-context-api-openapi.yml
  format: yaml
  label: Feason Context API
  slug: feason-com-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feason-com/openapi/feason-com-context-api-openapi.yml
- filename: feason-com-proof-api-openapi.yml
  format: yaml
  label: Feason Proof API
  slug: feason-com-proof-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feason-com/openapi/feason-com-proof-api-openapi.yml
- filename: feason-com-well-known-api-openapi.yml
  format: yaml
  label: Feason .well Known API
  slug: feason-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feason-com/openapi/feason-com-well-known-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Feason Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Feason declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Feason
provider_slug: feason-com
scheme_count: 1
schemes:
- evidence: 'curl --fail-with-body --connect-timeout 10 --max-time 20 \ https://www.feason.com/api/context/v1/contextualize \ -H "Authorization: Bearer $FEASON_CONTEXT_TOKEN" \ -H "Content-Type: application/json" \ --data ''{...}'''
  header: Authorization
  how_to_obtain: Create a scoped Context key via the Feason developer portal; the key is provided as a read‑only token to be set in the FEASON_CONTEXT_TOKEN environment variable.
  location: header
  name: Bearer
  type: http-bearer
slug: feason-com-authentication
source_filename: feason-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.feason.com/developers/quickstart
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.feason.com/developers/quickstart\nsources:\n- https://www.feason.com/developers/quickstart\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl --fail-with-body --connect-timeout 10 --max-time 20 \\ https://www.feason.com/api/context/v1/contextualize \\ -H \"Authorization:\n    Bearer $FEASON_CONTEXT_TOKEN\" \\ -H \"Content-Type: application/json\" \\ --data ''{...}'''\n  location: header\n  header: Authorization\n  how_to_obtain: Create a scoped Context key via the Feason developer portal; the key is provided as a read‑only token to be set in the FEASON_CONTEXT_TOKEN\n    environment variable.\ndocs: https://www.feason.com/developers/quickstart\n"
source_yaml_url: https://artifacts.apis.io/feason-com/authentication/feason-com-authentication.yml
summary_line: 1 scheme
tags:
- Scripture
- Courses
- Christian History
- Fellowship
- Prayer
---
