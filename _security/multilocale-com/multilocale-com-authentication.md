---
anonymous_access: false
api_key_in: []
api_specs:
- filename: multilocale-com-phrases-api-openapi.yml
  format: yaml
  label: MultiLocale Phrases API
  slug: multilocale-com-phrases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multilocale-com/openapi/multilocale-com-phrases-api-openapi.yml
- filename: multilocale-com-projects-api-openapi.yml
  format: yaml
  label: MultiLocale Projects API
  slug: multilocale-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multilocale-com/openapi/multilocale-com-projects-api-openapi.yml
- filename: multilocale-com-sandbox-api-openapi.yml
  format: yaml
  label: MultiLocale Sandbox API
  slug: multilocale-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multilocale-com/openapi/multilocale-com-sandbox-api-openapi.yml
auth_types: []
description: Authentication methods for Multilocale API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: MultiLocale Authentication
name_suffix: Authentication
oauth_flows: []
overview: MultiLocale declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: MultiLocale
provider_slug: multilocale-com
scheme_count: 2
schemes:
- evidence: 'API key — Authorization: Basic <base64(secret)> , for server-to-server integrations.'
  header: Authorization
  how_to_obtain: Create a key per project on app.multilocale.com; the secret is used directly in the Authorization header as "Basic <base64(secret)>".
  location: header
  name: API key
  scopes:
  - projects:read
  - projects:write
  - phrases:read
  - phrases:write
  - translations:write
  type: apiKey
- evidence: 'Access token — Authorization: Token <base64(accessToken)> , the JWT the dashboard and the CLI''s browser session use.'
  header: Authorization
  how_to_obtain: 'Obtain an access token by logging in (POST /api/login) or signing up (POST /api/signup) with email and password; the response includes an "accessToken" which is then sent as "Authorization: Token <base64(accessToken)>".'
  location: header
  name: Access token
  type: apiKey
slug: multilocale-com-authentication
source_filename: multilocale-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.multilocale.com/docs/api/authentication/
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.multilocale.com/docs/api/authentication/\nsources:\n- https://www.multilocale.com/docs/api/authentication/\n- https://www.multilocale.com/docs/api/authentication/\n- https://developers.multilocale.com/docs/api/authentication/\n- https://www.multilocale.com/docs/cli/getting-started/\ndescription: Authentication methods for Multilocale API\nschemes:\n- type: apiKey\n  name: API key\n  evidence: 'API key — Authorization: Basic <base64(secret)> , for server-to-server integrations.'\n  location: header\n  header: Authorization\n  scopes:\n  - projects:read\n  - projects:write\n  - phrases:read\n  - phrases:write\n  - translations:write\n  how_to_obtain: Create a key per project on app.multilocale.com; the secret is used directly in the Authorization header as \"Basic <base64(secret)>\".\n- type: apiKey\n  name: Access token\n  evidence: 'Access token — Authorization: Token\
  \ <base64(accessToken)> , the JWT the dashboard and the CLI''s browser session use.'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Obtain an access token by logging in (POST /api/login) or signing up (POST /api/signup) with email and password; the response\n    includes an \"accessToken\" which is then sent as \"Authorization: Token <base64(accessToken)>\".'\nnote: No OAuth2 flows are documented; authentication is performed via API keys or JWT access tokens sent in the Authorization header.\ndocs: https://www.multilocale.com/docs/api/authentication/\n"
source_yaml_url: https://artifacts.apis.io/multilocale-com/authentication/multilocale-com-authentication.yml
summary_line: 2 schemes
tags:
- Localization
- Translation
- Developer Tools
- Software-as-a-Service
---
