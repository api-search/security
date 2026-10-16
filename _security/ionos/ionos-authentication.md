---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ionos-openapi-generated.yml
  format: yaml
  label: IONOS API
  slug: ionos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ionos/refs/heads/main/openapi/_ae-authored/ionos-openapi-generated.yml
auth_types: []
description: Authentication methods for IONOS APIs as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ionos Authentication
name_suffix: Authentication
oauth_flows: []
overview: IONOS declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: IONOS
provider_slug: ionos
scheme_count: 3
schemes:
- evidence: 'All requests to the In-Memory DB v2 API require a Bearer token in the `Authorization` header:'
  header: Authorization
  how_to_obtain: Generate a token using the IONOS CLOUD Authentication API.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'All requests to the MariaDB API require a Bearer token in the `Authorization` header:'
  header: Authorization
  how_to_obtain: Generate a token using the IONOS CLOUD Authentication API.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: '### Basic Authentication * **Type**: HTTP basic authentication'
  header: Authorization
  how_to_obtain: Provide `IONOS_USERNAME` and `IONOS_PASSWORD` environment variables or pass them to the SDK configuration.
  location: header
  name: Basic Authentication (SDK)
  type: http-basic
slug: ionos-authentication
source_filename: ionos-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ionos.com/cloud/ai/mcp-server/configuration/authentication.md
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ionos.com/cloud/ai/mcp-server/configuration/authentication.md\nsources:\n- https://docs.ionos.com/cloud/ai/mcp-server/configuration/authentication.md\n- https://docs.ionos.com/cloud/api-reference/databases/v2/authentication.md\n- https://docs.ionos.com/cloud/api-reference/databases/v2-1/authentication.md\n- https://docs.ionos.com/cloud/go/go-bundle/sdks/auth.md\ndescription: Authentication methods for IONOS APIs as documented.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'All requests to the In-Memory DB v2 API require a Bearer token in the `Authorization` header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a token using the IONOS CLOUD Authentication API.\n- type: http-bearer\n  name: Bearer token\n  evidence: 'All requests to the MariaDB API require a Bearer token in the `Authorization` header:'\n  location: header\n\
  \  header: Authorization\n  how_to_obtain: Generate a token using the IONOS CLOUD Authentication API.\n- type: http-basic\n  name: Basic Authentication (SDK)\n  evidence: '### Basic Authentication * **Type**: HTTP basic authentication'\n  location: header\n  header: Authorization\n  how_to_obtain: Provide `IONOS_USERNAME` and `IONOS_PASSWORD` environment variables or pass them to the SDK configuration.\ndocs: https://docs.ionos.com/cloud/ai/mcp-server/configuration/authentication.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ionos/refs/heads/main/authentication/ionos-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Cloud
- Hosting
- Domains
- AI
---
