---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mnemoverse-com-health-api-openapi.yml
  format: yaml
  label: Mnemoverse Health API
  slug: mnemoverse-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mnemoverse-com/openapi/mnemoverse-com-health-api-openapi.yml
- filename: mnemoverse-com-memory-api-openapi.yml
  format: yaml
  label: Mnemoverse Memory API
  slug: mnemoverse-com-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mnemoverse-com/openapi/mnemoverse-com-memory-api-openapi.yml
- filename: mnemoverse-com-memory-v1-api-openapi.yml
  format: yaml
  label: Mnemoverse Memory V1 API
  slug: mnemoverse-com-memory-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mnemoverse-com/openapi/mnemoverse-com-memory-v1-api-openapi.yml
- filename: mnemoverse-com-vault-api-openapi.yml
  format: yaml
  label: Mnemoverse Vault API
  slug: mnemoverse-com-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mnemoverse-com/openapi/mnemoverse-com-vault-api-openapi.yml
auth_types: []
description: Authentication methods for Mnemoverse API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mnemoverse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mnemoverse declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Mnemoverse
provider_slug: mnemoverse-com
scheme_count: 2
schemes:
- evidence: 'All /memory/* endpoints require authentication via X-Api-Key header or Authorization: Bearer header.'
  header: X-Api-Key
  how_to_obtain: Obtain an API key from the Mnemoverse console and include it in the X-Api-Key header.
  location: header
  name: X-Api-Key
  type: apiKey
- evidence: 'All /memory/* endpoints require authentication via X-Api-Key header or Authorization: Bearer header.'
  header: Authorization
  how_to_obtain: Use the same API key as a Bearer token in the Authorization header.
  location: header
  name: Authorization
  type: http-bearer
slug: mnemoverse-com-authentication
source_filename: mnemoverse-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mnemoverse.com/docs/api/reference
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mnemoverse.com/docs/api/reference\nsources:\n- https://mnemoverse.com/docs/api/reference\n- https://mnemoverse.com/docs/api/remote-mcp-server\n- https://mnemoverse.com/docs/api/shared-api-key\n- https://mnemoverse.com/docs/library/memory-poisoning-secret-leak\ndescription: Authentication methods for Mnemoverse API\nschemes:\n- type: apiKey\n  name: X-Api-Key\n  evidence: 'All /memory/* endpoints require authentication via X-Api-Key header or Authorization: Bearer header.'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Obtain an API key from the Mnemoverse console and include it in the X-Api-Key header.\n- type: http-bearer\n  name: Authorization\n  evidence: 'All /memory/* endpoints require authentication via X-Api-Key header or Authorization: Bearer header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Use the same API key as a Bearer token\
  \ in the Authorization header.\ndocs: https://mnemoverse.com/docs/api/reference\n"
source_yaml_url: https://artifacts.apis.io/mnemoverse-com/authentication/mnemoverse-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Memory
- Persistent
---
