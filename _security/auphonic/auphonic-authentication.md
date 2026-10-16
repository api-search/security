---
anonymous_access: false
api_key_in: []
api_specs:
- filename: auphonic-info-api-openapi.yml
  format: yaml
  label: Auphonic Info API
  slug: auphonic-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-info-api-openapi.yml
- filename: auphonic-presets-api-openapi.yml
  format: yaml
  label: Auphonic Presets API
  slug: auphonic-presets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-presets-api-openapi.yml
- filename: auphonic-productions-api-openapi.yml
  format: yaml
  label: Auphonic Productions API
  slug: auphonic-productions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-productions-api-openapi.yml
- filename: auphonic-services-api-openapi.yml
  format: yaml
  label: Auphonic Services API
  slug: auphonic-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-services-api-openapi.yml
- filename: auphonic-simple-api-api-openapi.yml
  format: yaml
  label: Auphonic Simple API
  slug: auphonic-simple-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-simple-api-api-openapi.yml
- filename: auphonic-user-api-openapi.yml
  format: yaml
  label: Auphonic User API
  slug: auphonic-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-user-api-openapi.yml
auth_types: []
description: Authentication methods for Auphonic API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Auphonic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Auphonic declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Auphonic
provider_slug: auphonic
scheme_count: 3
schemes:
- evidence: 'Add the API Key to the authorization header: curl https://auphonic.com/api/productions.json -H "Authorization: bearer {api_key}" or to a GET parameter (for streaming audio files, loading pictures, etc.): curl https://auphonic.com/api/productions.json?bearer_token={api_key}'
  header: Authorization
  how_to_obtain: Create and revoke API Keys on the Account Settings Page.
  location: header
  name: API Key
  type: apiKey
- evidence: 'Alternatively to API Key Authentication, you can access all API resources using your auphonic username and password. An example which returns all your productions: curl https://auphonic.com/api/productions.json -u username:password'
  how_to_obtain: Use your Auphonic username and password.
  location: header
  name: HTTP Basic
  type: http-basic
- authorize_url: https://auphonic.com/oauth2/authorize/?client_id={client_id}&redirect_uri={redirect_uri}&response_type=code
  evidence: Auphonic authentication primarly uses OAuth 2.0, as an easy way to authenticate third party applications.
  header: Authorization
  how_to_obtain: Register an Auphonic App to obtain a client ID and secret, then follow the appropriate OAuth flow (authorization_code for web apps or password for desktop/mobile apps).
  location: header
  name: OAuth 2.0
  token_url: https://auphonic.com/oauth2/token/
  type: oauth2
slug: auphonic-authentication
source_filename: auphonic-authentication.yml
source_heading: Authentication Profile
source_url: https://auphonic.com/help/api/authentication.html
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://auphonic.com/help/api/authentication.html\nsources:\n- https://auphonic.com/help/api/authentication.html\ndescription: Authentication methods for Auphonic API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Add the API Key to the authorization header: curl https://auphonic.com/api/productions.json -H \"Authorization: bearer {api_key}\"\n    or to a GET parameter (for streaming audio files, loading pictures, etc.): curl https://auphonic.com/api/productions.json?bearer_token={api_key}'\n  location: header\n  header: Authorization\n  how_to_obtain: Create and revoke API Keys on the Account Settings Page.\n- type: http-basic\n  name: HTTP Basic\n  evidence: 'Alternatively to API Key Authentication, you can access all API resources using your auphonic username and password. An example which\n    returns all your productions: curl https://auphonic.com/api/productions.json\
  \ -u username:password'\n  location: header\n  how_to_obtain: Use your Auphonic username and password.\n- type: oauth2\n  name: OAuth 2.0\n  evidence: Auphonic authentication primarly uses OAuth 2.0, as an easy way to authenticate third party applications.\n  location: header\n  header: Authorization\n  token_url: https://auphonic.com/oauth2/token/\n  authorize_url: https://auphonic.com/oauth2/authorize/?client_id={client_id}&redirect_uri={redirect_uri}&response_type=code\n  how_to_obtain: Register an Auphonic App to obtain a client ID and secret, then follow the appropriate OAuth flow (authorization_code for web\n    apps or password for desktop/mobile apps).\ndocs: https://auphonic.com/help/api/authentication.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/authentication/auphonic-authentication.yml
summary_line: 3 schemes
tags:
- Audio
- Podcasting
- AI
- Automation
- Media
---
