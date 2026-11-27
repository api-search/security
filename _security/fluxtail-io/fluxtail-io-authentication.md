---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fluxtail-io-facets-api-openapi.yml
  format: yaml
  label: Fluxtail Facets API
  slug: fluxtail-io-facets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxtail-io/openapi/fluxtail-io-facets-api-openapi.yml
- filename: fluxtail-io-histogram-api-openapi.yml
  format: yaml
  label: Fluxtail Histogram API
  slug: fluxtail-io-histogram-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxtail-io/openapi/fluxtail-io-histogram-api-openapi.yml
- filename: fluxtail-io-logs-api-openapi.yml
  format: yaml
  label: Fluxtail Logs API
  slug: fluxtail-io-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxtail-io/openapi/fluxtail-io-logs-api-openapi.yml
- filename: fluxtail-io-receivers-api-openapi.yml
  format: yaml
  label: Fluxtail Receivers API
  slug: fluxtail-io-receivers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxtail-io/openapi/fluxtail-io-receivers-api-openapi.yml
auth_types: []
description: Authentication schemes for Fluxtail as documented.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fluxtail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fluxtail declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fluxtail
provider_slug: fluxtail-io
scheme_count: 1
schemes:
- evidence: A shared request must provide one valid receiver-bound Bearer token.
  header: Authorization
  how_to_obtain: Create a token in the Access tokens page, select the required scopes, and bind ingest:write to the intended receiver.
  location: header
  name: Shared receiver Bearer token
  scopes:
  - ingest:write
  - logs:read
  - analytics:read
  type: http-bearer
slug: fluxtail-io-authentication
source_filename: fluxtail-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.fluxtail.io/troubleshooting/authentication-and-limits/
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.fluxtail.io/troubleshooting/authentication-and-limits/\nsources:\n- https://docs.fluxtail.io/troubleshooting/authentication-and-limits/\n- https://docs.fluxtail.io/route/access-tokens/\n- https://docs.fluxtail.io/getting-started/first-log/\n- https://docs.fluxtail.io/getting-started/core-concepts/\ndescription: Authentication schemes for Fluxtail as documented.\nschemes:\n- type: http-bearer\n  name: Shared receiver Bearer token\n  evidence: A shared request must provide one valid receiver-bound Bearer token.\n  location: header\n  header: Authorization\n  scopes:\n  - ingest:write\n  - logs:read\n  - analytics:read\n  how_to_obtain: Create a token in the Access tokens page, select the required scopes, and bind ingest:write to the intended receiver.\ndocs: https://docs.fluxtail.io/troubleshooting/authentication-and-limits/\n"
source_yaml_url: https://artifacts.apis.io/fluxtail-io/authentication/fluxtail-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Logging
- Centralized
- MCP
- Artificial Intelligence
---
