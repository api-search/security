---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sgpdirectory-com-api-openapi.json
  format: json
  label: SGP Directory API API
  slug: sgp-directory-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sgpdirectory-com/openapi/_original/sgpdirectory-com-api-openapi.json
auth_types: []
description: Authentication uses an API key passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Sgpdirectory Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: sgpdirectory-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: sgpdirectory-com
provider_slug: sgpdirectory-com
scheme_count: 1
schemes:
- evidence: 'curl "https://api.sgpdirectory.com/v1/entities/197501035Z/officers" \ -H "Authorization: Bearer YOUR-API-KEY"'
  header: Authorization
  how_to_obtain: Obtain a free API key from the Console (console.sgpdirectory.com) under API Keys → Create Key. The key starts with sgpd_.
  location: header
  name: Bearer
  type: http-bearer
slug: sgpdirectory-com-authentication
source_filename: sgpdirectory-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.sgpdirectory.com/docs/quickstart
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.sgpdirectory.com/docs/quickstart\nsources:\n- https://docs.sgpdirectory.com/docs/quickstart\n- https://docs.sgpdirectory.com/docs/mcp/setup\ndescription: Authentication uses an API key passed as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl \"https://api.sgpdirectory.com/v1/entities/197501035Z/officers\" \\ -H \"Authorization: Bearer YOUR-API-KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a free API key from the Console (console.sgpdirectory.com) under API Keys → Create Key. The key starts with sgpd_.\nnote: No OAuth2, apiKey, or other authentication schemes are documented.\ndocs: https://docs.sgpdirectory.com/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/sgpdirectory-com/authentication/sgpdirectory-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Directory
- Singapore
- Business
- API
---
