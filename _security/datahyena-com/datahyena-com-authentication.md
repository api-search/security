---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datahyena-com-acquisitions-api-openapi.yml
  format: yaml
  label: datahyena-com Acquisitions API
  slug: datahyena-com-acquisitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datahyena-com/openapi/datahyena-com-acquisitions-api-openapi.yml
- filename: datahyena-com-companies-api-openapi.yml
  format: yaml
  label: datahyena-com Companies API
  slug: datahyena-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datahyena-com/openapi/datahyena-com-companies-api-openapi.yml
- filename: datahyena-com-exec-moves-api-openapi.yml
  format: yaml
  label: datahyena-com Exec Moves API
  slug: datahyena-com-exec-moves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datahyena-com/openapi/datahyena-com-exec-moves-api-openapi.yml
- filename: datahyena-com-funding-events-api-openapi.yml
  format: yaml
  label: datahyena-com Funding Events API
  slug: datahyena-com-funding-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datahyena-com/openapi/datahyena-com-funding-events-api-openapi.yml
- filename: datahyena-com-hiring-signals-api-openapi.yml
  format: yaml
  label: datahyena-com Hiring Signals API
  slug: datahyena-com-hiring-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datahyena-com/openapi/datahyena-com-hiring-signals-api-openapi.yml
- filename: datahyena-com-investors-api-openapi.yml
  format: yaml
  label: datahyena-com Investors API
  slug: datahyena-com-investors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datahyena-com/openapi/datahyena-com-investors-api-openapi.yml
auth_types: []
description: Authentication methods for Datahyena API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Datahyena Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: datahyena-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: datahyena-com
provider_slug: datahyena-com
scheme_count: 2
schemes:
- evidence: 'Send it in the `X-API-Key` header on every request:'
  header: X-API-Key
  how_to_obtain: The user issues it from the dashboard at https://app.datahyena.com and supplies it through a secure channel (environment variable DATAHYENA_API_KEY).
  location: header
  name: API Key
  type: apiKey
- evidence: 'Authentication is OAuth 2.1 with PKCE: the user signs in and approves read scopes in the browser'
  how_to_obtain: The user completes a browser OAuth flow; the MCP client obtains a token without the user exposing credentials.
  name: OAuth 2.1 with PKCE (MCP)
  scopes:
  - read:funding
  - read:acquisitions
  - read:exec_moves
  - read:companies
  - read:investors
  type: oauth2
slug: datahyena-com-authentication
source_filename: datahyena-com-authentication.yml
source_heading: Authentication Profile
source_url: https://datahyena.com/auth.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://datahyena.com/auth.md\nsources:\n- https://datahyena.com/auth.md\n- https://datahyena.com/docs/guides/quick-start/\ndescription: Authentication methods for Datahyena API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Send it in the `X-API-Key` header on every request:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: The user issues it from the dashboard at https://app.datahyena.com and supplies it through a secure channel (environment variable\n    DATAHYENA_API_KEY).\n- type: oauth2\n  name: OAuth 2.1 with PKCE (MCP)\n  evidence: 'Authentication is OAuth 2.1 with PKCE: the user signs in and approves read scopes in the browser'\n  scopes:\n  - read:funding\n  - read:acquisitions\n  - read:exec_moves\n  - read:companies\n  - read:investors\n  how_to_obtain: The user completes a browser OAuth flow; the MCP client obtains a token without the user exposing\
  \ credentials.\ndocs: https://datahyena.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/datahyena-com/authentication/datahyena-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data
- Funding
- M&A
- Hiring
- API
---
