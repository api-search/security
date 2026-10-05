---
anonymous_access: false
api_key_in: []
api_specs:
- filename: qlik-apps-api-openapi.yml
  format: yaml
  label: Qlik Apps API
  slug: qlik-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik/refs/heads/main/openapi/qlik-apps-api-openapi.yml
- filename: qlik-evaluation-api-openapi.yml
  format: yaml
  label: Qlik Evaluation API
  slug: qlik-evaluation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik/refs/heads/main/openapi/qlik-evaluation-api-openapi.yml
- filename: qlik-filters-api-openapi.yml
  format: yaml
  label: Qlik Filters API
  slug: qlik-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik/refs/heads/main/openapi/qlik-filters-api-openapi.yml
- filename: qlik-insight-analyses-api-openapi.yml
  format: yaml
  label: Qlik Insight Analyses API
  slug: qlik-insight-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik/refs/heads/main/openapi/qlik-insight-analyses-api-openapi.yml
auth_types: []
description: Authentication methods for Qlik REST APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Qlik Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qlik declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Qlik
provider_slug: qlik
scheme_count: 2
schemes:
- evidence: 'curl "https://{tenant}.{region}.qlikcloud.com/api/v1/api-keys" \ -H "Authorization: Bearer <access_token>"'
  header: Authorization
  how_to_obtain: Create an API key via the API keys endpoint; the response includes a signed JWT token to be used as a Bearer token.
  location: header
  name: API Key Bearer Token
  type: http-bearer
- evidence: 'curl "https://{tenant}.{region}.qlikcloud.com/api/v1/oauth-tokens" \ -H "Authorization: Bearer <access_token>"'
  header: Authorization
  how_to_obtain: Obtain an access token via the OAuth token endpoint (POST /oauth/token) using an appropriate grant type.
  location: header
  name: OAuth Access Token
  type: http-bearer
slug: qlik-authentication
source_filename: qlik-authentication.yml
source_heading: Authentication Profile
source_url: https://qlik.dev/apis/rest/api-keys/
source_yaml: "generated: '2026-10-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://qlik.dev/apis/rest/api-keys/\nsources:\n- https://qlik.dev/apis/rest/api-keys/\n- https://qlik.dev/apis/rest/oauth/\n- https://qlik.dev/apis/rest/oauth-clients/\n- https://qlik.dev/apis/rest/oauth-tokens/\ndescription: Authentication methods for Qlik REST APIs\nschemes:\n- type: http-bearer\n  name: API Key Bearer Token\n  evidence: 'curl \"https://{tenant}.{region}.qlikcloud.com/api/v1/api-keys\" \\ -H \"Authorization: Bearer <access_token>\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key via the API keys endpoint; the response includes a signed JWT token to be used as a Bearer token.\n- type: http-bearer\n  name: OAuth Access Token\n  evidence: 'curl \"https://{tenant}.{region}.qlikcloud.com/api/v1/oauth-tokens\" \\ -H \"Authorization: Bearer <access_token>\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain an access\
  \ token via the OAuth token endpoint (POST /oauth/token) using an appropriate grant type.\ndocs: https://qlik.dev/apis/rest/api-keys/\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qlik/refs/heads/main/authentication/qlik-authentication.yml
summary_line: 2 schemes
tags:
- Security
- Access Control
- Machine Learning
- Artificial Intelligence
- Analytics
- Data Integration
- Cloud
---
