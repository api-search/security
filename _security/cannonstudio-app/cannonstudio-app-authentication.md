---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cannonstudio-app-openapi-generated.yml
  format: yaml
  label: Cannon Studio API
  slug: cannonstudio-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cannonstudio-app/openapi/_ae-authored/cannonstudio-app-openapi-generated.yml
auth_types: []
description: Cannon Studio API authentication uses API keys.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cannonstudio App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cannon Studio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cannon Studio
provider_slug: cannonstudio-app
scheme_count: 2
schemes:
- evidence: Keys can be used in the `x-api-key` header or as a bearer token.
  header: x-api-key
  how_to_obtain: Create keys from the developer console under API Keys.
  location: header
  name: x-api-key
  type: apiKey
- evidence: 'Authorization: Bearer cs_live_... Supported if your existing client stack expects bearer auth.'
  header: Authorization
  how_to_obtain: Create keys from the developer console under API Keys.
  location: header
  name: Authorization
  type: http-bearer
slug: cannonstudio-app-authentication
source_filename: cannonstudio-app-authentication.yml
source_heading: Authentication Profile
source_url: https://www.cannonstudio.app/developers/docs/authentication
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.cannonstudio.app/developers/docs/authentication\nsources:\n- https://www.cannonstudio.app/developers/docs/authentication\n- https://www.cannonstudio.app/developers/docs/reference/status\n- https://www.cannonstudio.app/developers/docs/quickstart\n- https://www.cannonstudio.app/developers/docs/reference/create-request\ndescription: Cannon Studio API authentication uses API keys.\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: Keys can be used in the `x-api-key` header or as a bearer token.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create keys from the developer console under API Keys.\n- type: http-bearer\n  name: Authorization\n  evidence: 'Authorization: Bearer cs_live_... Supported if your existing client stack expects bearer auth.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys from the developer console under\
  \ API Keys.\nnote: No OAuth2, JWT, HMAC, MTLS, or other authentication schemes are documented.\ndocs: https://www.cannonstudio.app/developers/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/cannonstudio-app/authentication/cannonstudio-app-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Video Production
- Advertising
- Content Creation
- Multimedia
---
