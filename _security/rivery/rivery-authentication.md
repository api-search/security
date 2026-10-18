---
anonymous_access: false
api_key_in: []
api_specs:
- filename: rivery-accounts-api-openapi.yml
  format: yaml
  label: Rivery Accounts API
  slug: rivery-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/openapi/rivery-accounts-api-openapi.yml
- filename: rivery-activities-api-openapi.yml
  format: yaml
  label: Rivery Activities API
  slug: rivery-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/openapi/rivery-activities-api-openapi.yml
- filename: rivery-audit-events-api-openapi.yml
  format: yaml
  label: Rivery Audit Events API
  slug: rivery-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/openapi/rivery-audit-events-api-openapi.yml
- filename: rivery-connections-api-openapi.yml
  format: yaml
  label: Rivery Connections API
  slug: rivery-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/openapi/rivery-connections-api-openapi.yml
- filename: rivery-data-flows-metadata-api-openapi.yml
  format: yaml
  label: Rivery Data Flows Metadata API
  slug: rivery-data-flows-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/openapi/rivery-data-flows-metadata-api-openapi.yml
- filename: rivery-dataframes-api-openapi.yml
  format: yaml
  label: Rivery Dataframes API
  slug: rivery-dataframes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/openapi/rivery-dataframes-api-openapi.yml
- filename: rivery-environments-api-openapi.yml
  format: yaml
  label: Rivery Environments API
  slug: rivery-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/openapi/rivery-environments-api-openapi.yml
- filename: rivery-logicode-api-openapi.yml
  format: yaml
  label: Rivery Logicode API
  slug: rivery-logicode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/openapi/rivery-logicode-api-openapi.yml
- filename: rivery-mcp-api-openapi.yml
  format: yaml
  label: Rivery MCP API
  slug: rivery-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/openapi/rivery-mcp-api-openapi.yml
- filename: rivery-operations-api-openapi.yml
  format: yaml
  label: Rivery Operations API
  slug: rivery-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/openapi/rivery-operations-api-openapi.yml
- filename: rivery-river-source-api-openapi.yml
  format: yaml
  label: Rivery River Source API
  slug: rivery-river-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/openapi/rivery-river-source-api-openapi.yml
- filename: rivery-users-api-openapi.yml
  format: yaml
  label: Rivery Users API
  slug: rivery-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/openapi/rivery-users-api-openapi.yml
- filename: rivery-variables-api-openapi.yml
  format: yaml
  label: Rivery Variables API
  slug: rivery-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/openapi/rivery-variables-api-openapi.yml
- filename: rivery-dataflows-api-openapi.yml
  format: yaml
  label: Rivery Dataflows API
  slug: rivery-dataflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/openapi/rivery-dataflows-api-openapi.yml
auth_types: []
description: Authentication methods supported by Boomi Data Integration
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Rivery Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rivery declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Rivery
provider_slug: rivery
scheme_count: 4
schemes:
- evidence: 'Bearer token authentication sends a token in the Authorization: Bearer <token> header.'
  header: Authorization
  location: header
  name: Bearer token
  type: http-bearer
- evidence: Use Basic HTTP authentication to send a Base64-encoded username and password in the Authorization header.
  header: Authorization
  location: header
  name: Basic HTTP
  type: http-basic
- evidence: The system appends the key to the request URL as a query parameter.
  location: query
  name: API key (query)
  type: apiKey
- evidence: Client credentials grant Server-to-server authentication where your application authenticates directly without user involvement.
  flows:
  - client_credentials
  how_to_obtain: Provide client_id and client_secret (optionally sent as Basic Auth header).
  name: OAuth2 client_credentials
  token_url: https://auth.example.com/oauth2/token
  type: oauth2
slug: rivery-authentication
source_filename: rivery-authentication.yml
source_heading: Authentication Profile
source_url: https://help.boomi.com/docs/Atomsphere/Data_Integration/Blueprint/authentication-methods
source_yaml: "generated: '2026-10-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.boomi.com/docs/Atomsphere/Data_Integration/Blueprint/authentication-methods\nsources:\n- https://help.boomi.com/docs/Atomsphere/Data_Integration/Blueprint/authentication-methods\n- https://help.boomi.com/docs/Atomsphere/Data_Integration/Sources/Applications/refreshing-credentials-in-an-existing-oauth2-connection\n- https://help.boomi.com/docs/Atomsphere/Platform/quickstart_guides\n- https://help.boomi.com/docs/Atomsphere/Orchestrate/Getting_started_with_Orchestrate/orchestrate_overview\ndescription: Authentication methods supported by Boomi Data Integration\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Bearer token authentication sends a token in the Authorization: Bearer <token> header.'\n  location: header\n  header: Authorization\n- type: http-basic\n  name: Basic HTTP\n  evidence: Use Basic HTTP authentication to send a Base64-encoded username\
  \ and password in the Authorization header.\n  location: header\n  header: Authorization\n- type: apiKey\n  name: API key (query)\n  evidence: The system appends the key to the request URL as a query parameter.\n  location: query\n- type: oauth2\n  name: OAuth2 client_credentials\n  evidence: Client credentials grant Server-to-server authentication where your application authenticates directly without user involvement.\n  flows:\n  - client_credentials\n  token_url: https://auth.example.com/oauth2/token\n  how_to_obtain: Provide client_id and client_secret (optionally sent as Basic Auth header).\ndocs: https://help.boomi.com/docs/Atomsphere/Data_Integration/Blueprint/authentication-methods\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rivery/refs/heads/main/authentication/rivery-authentication.yml
summary_line: 4 schemes
tags:
- Data Integration
- ELT
- Cloud
- Low-code
- Boomi
---
