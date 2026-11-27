---
anonymous_access: false
api_key_in: []
api_specs:
- filename: osir-com-openapi-generated.yml
  format: yaml
  label: OSIR API
  slug: osir-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osir-com/openapi/_ae-authored/osir-com-openapi-generated.yml
auth_types: []
description: Authentication methods for OSIR API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: OSIR Authentication
name_suffix: Authentication
oauth_flows: []
overview: OSIR declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: OSIR
provider_slug: osir-com
scheme_count: 3
schemes:
- evidence: 'curl -H "Authorization: Bearer osir_live_xxx" \ https://be.osir.com/v1/public/catalog/domains/example.com/availability'
  header: Authorization
  how_to_obtain: Create an API key in the OSIR panel (Settings > API Keys) and copy the key.
  location: header
  name: API Key Bearer Token
  type: http-bearer
- evidence: 'curl -X GET https://be.osir.com/v1/public/catalog/domains/example.com/availability \ -H "X-API-Key: osir_live_your_api_key"'
  header: X-API-Key
  how_to_obtain: Create an API key in the OSIR panel (Settings > API Keys) and copy the key.
  location: header
  name: X-API-Key Header
  type: apiKey
- authorize_url: https://osir.com/oauth/authorize?
  evidence: 'Step 1: Redirect to Authorization https://osir.com/oauth/authorize?client_id=your_client_id&redirect_uri=https://yourapp.com/callback&response_type=code&scope=domains:read domains:write'
  flows:
  - authorization_code
  how_to_obtain: Register an application with OSIR to receive a client_id and client_secret, then follow the OAuth authorization code flow.
  name: OAuth 2.0
  scopes:
  - domains:read
  - domains:write
  - vps:read
  - vps:write
  - email:read
  - email:write
  - billing:read
  - billing:write
  type: oauth2
slug: osir-com-authentication
source_filename: osir-com-authentication.yml
source_heading: Authentication Profile
source_url: https://osir.com/en/help/managing-api-keys/
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://osir.com/en/help/managing-api-keys/\nsources:\n- https://osir.com/en/help/managing-api-keys/\n- https://osir.com/en/help/api-authentication/\n- https://osir.com/en/help/two-factor-authentication/\n- https://osir.com/en/help/fossbilling-setup/\ndescription: Authentication methods for OSIR API\nschemes:\n- type: http-bearer\n  name: API Key Bearer Token\n  evidence: 'curl -H \"Authorization: Bearer osir_live_xxx\" \\ https://be.osir.com/v1/public/catalog/domains/example.com/availability'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the OSIR panel (Settings > API Keys) and copy the key.\n- type: apiKey\n  name: X-API-Key Header\n  evidence: 'curl -X GET https://be.osir.com/v1/public/catalog/domains/example.com/availability \\ -H \"X-API-Key: osir_live_your_api_key\"'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an\
  \ API key in the OSIR panel (Settings > API Keys) and copy the key.\n- type: oauth2\n  name: OAuth 2.0\n  evidence: 'Step 1: Redirect to Authorization https://osir.com/oauth/authorize?client_id=your_client_id&redirect_uri=https://yourapp.com/callback&response_type=code&scope=domains:read\n    domains:write'\n  flows:\n  - authorization_code\n  authorize_url: https://osir.com/oauth/authorize?\n  scopes:\n  - domains:read\n  - domains:write\n  - vps:read\n  - vps:write\n  - email:read\n  - email:write\n  - billing:read\n  - billing:write\n  how_to_obtain: Register an application with OSIR to receive a client_id and client_secret, then follow the OAuth authorization code flow.\ndocs: https://osir.com/en/help/managing-api-keys/\n"
source_yaml_url: https://artifacts.apis.io/osir-com/authentication/osir-com-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Domain Registrar
- Automation
- Hosting
---
