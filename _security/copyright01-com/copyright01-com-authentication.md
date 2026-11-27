---
anonymous_access: false
api_key_in: []
api_specs:
- filename: copyright01-com-api-keys-api-openapi.yml
  format: yaml
  label: Copyright01 Api Keys API
  slug: copyright01-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/copyright01-com/openapi/copyright01-com-api-keys-api-openapi.yml
- filename: copyright01-com-deposits-api-openapi.yml
  format: yaml
  label: Copyright01 Deposits API
  slug: copyright01-com-deposits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/copyright01-com/openapi/copyright01-com-deposits-api-openapi.yml
- filename: copyright01-com-me-api-openapi.yml
  format: yaml
  label: Copyright01 Me API
  slug: copyright01-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/copyright01-com/openapi/copyright01-com-me-api-openapi.yml
- filename: copyright01-com-verify-api-openapi.yml
  format: yaml
  label: Copyright01 Verify API
  slug: copyright01-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/copyright01-com/openapi/copyright01-com-verify-api-openapi.yml
- filename: copyright01-com-verify-hash-api-openapi.yml
  format: yaml
  label: Copyright01 Verify Hash API
  slug: copyright01-com-verify-hash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/copyright01-com/openapi/copyright01-com-verify-hash-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Copyright01 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Copyright01 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Copyright01
provider_slug: copyright01-com
scheme_count: 1
schemes:
- description: 'API key as Bearer token. Create keys at https://copyright01.com/profil#api-keys. Example: Authorization: Bearer sk_your_api_key_here'
  key_management: API keys are created at https://copyright01.com/profil#api-keys (max 10 keys).
  key_prefix: sk_
  mcp: MCP server https://copyright01.com/mcp uses the same Bearer token (API key in Authorization header); verify_certificate is documented as public, no auth.
  name: ApiKeyAuth
  public_operations:
  - verifyCertificate
  scheme: bearer
  sources:
  - openapi/copyright01-com-openapi.yml
  - https://copyright01.com/llms-full.txt
  - https://copyright01.com/en/developers
  type: http
slug: copyright01-com-authentication
source_filename: copyright01-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://copyright01.com/llms-full.txt\ndocs: https://copyright01.com/en/developers\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: 'API key as Bearer token. Create keys at https://copyright01.com/profil#api-keys.\n    Example: Authorization: Bearer sk_your_api_key_here'\n  key_prefix: sk_\n  key_management: 'API keys are created at https://copyright01.com/profil#api-keys (max 10 keys).'\n  public_operations:\n  - verifyCertificate\n  mcp: 'MCP server https://copyright01.com/mcp uses the same Bearer token (API key in Authorization header); verify_certificate is documented as public, no auth.'\n  sources:\n  - openapi/copyright01-com-openapi.yml\n  - https://copyright01.com/llms-full.txt\n  - https://copyright01.com/en/developers\n"
source_yaml_url: https://artifacts.apis.io/copyright01-com/authentication/copyright01-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Copyright
- Intellectual Property
- Timestamping
- Proof Of Authorship
- Certificates
- MCP
- REST API
---
