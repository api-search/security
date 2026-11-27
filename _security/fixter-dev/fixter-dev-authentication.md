---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fixter-dev-openapi-generated.yml
  format: yaml
  label: Fixter API
  slug: fixter-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixter-dev/openapi/_ae-authored/fixter-dev-openapi-generated.yml
auth_types: []
description: Authentication schemes supported by Fixter API tests
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Fixter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fixter declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Fixter
provider_slug: fixter-dev
scheme_count: 5
schemes:
- evidence: 'BASIC Basic auth Authorization: Basic <base64(username:password)>'
  header: Authorization
  location: header
  name: BASIC
  type: http-basic
- evidence: 'BEARER Bearer token Authorization: Bearer <token>'
  header: Authorization
  location: header
  name: BEARER
  type: http-bearer
- evidence: 'API_KEY API key A custom header such as X-Api-Key: abc123 , or a query parameter such as ?api_key=abc123 , with the key as its value'
  header: X-Api-Key
  location: header
  name: API_KEY (header)
  type: apiKey
- evidence: 'API_KEY API key A custom header such as X-Api-Key: abc123 , or a query parameter such as ?api_key=abc123 , with the key as its value'
  header: api_key
  location: query
  name: API_KEY (query)
  type: apiKey
- evidence: 'OAUTH2_CLIENT_CREDENTIALS OAuth2 (client credentials) Authorization: Bearer <access token> , with the token fetched from your token URL'
  header: Authorization
  how_to_obtain: Fixter fetches the access token before it runs the test. The token request is a form POST to the token URL with grant_type=client_credentials, client_id and client_secret, plus scope and audience when they are set.
  location: header
  name: OAUTH2_CLIENT_CREDENTIALS
  token_url: tokenUrl
  type: oauth2
slug: fixter-dev-authentication
source_filename: fixter-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.fixter.dev/api-testing/credentials/
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.fixter.dev/api-testing/credentials/\nsources:\n- https://docs.fixter.dev/api-testing/credentials/\n- https://docs.fixter.dev/getting-started/introduction/\n- https://docs.fixter.dev/getting-started/onboarding/\n- https://docs.fixter.dev/setup/overview/\ndescription: Authentication schemes supported by Fixter API tests\nschemes:\n- type: http-basic\n  name: BASIC\n  evidence: 'BASIC Basic auth Authorization: Basic <base64(username:password)>'\n  location: header\n  header: Authorization\n- type: http-bearer\n  name: BEARER\n  evidence: 'BEARER Bearer token Authorization: Bearer <token>'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: API_KEY (header)\n  evidence: 'API_KEY API key A custom header such as X-Api-Key: abc123 , or a query parameter such as ?api_key=abc123 , with the key as its value'\n  location: header\n  header: X-Api-Key\n- type:\
  \ apiKey\n  name: API_KEY (query)\n  evidence: 'API_KEY API key A custom header such as X-Api-Key: abc123 , or a query parameter such as ?api_key=abc123 , with the key as its value'\n  location: query\n  header: api_key\n- type: oauth2\n  name: OAUTH2_CLIENT_CREDENTIALS\n  evidence: 'OAUTH2_CLIENT_CREDENTIALS OAuth2 (client credentials) Authorization: Bearer <access token> , with the token fetched from your token\n    URL'\n  location: header\n  header: Authorization\n  token_url: tokenUrl\n  how_to_obtain: Fixter fetches the access token before it runs the test. The token request is a form POST to the token URL with grant_type=client_credentials,\n    client_id and client_secret, plus scope and audience when they are set.\ndocs: https://docs.fixter.dev/api-testing/credentials/\n"
source_yaml_url: https://artifacts.apis.io/fixter-dev/authentication/fixter-dev-authentication.yml
summary_line: 5 schemes
tags:
- Monitoring
- Artificial Intelligence
- APM
- Error Tracking
- MCP
---
