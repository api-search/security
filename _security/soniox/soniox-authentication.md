---
anonymous_access: false
api_key_in: []
auth_types: []
description: Soniox uses an API key sent as a Bearer token in the Authorization header for both long‑lived and temporary keys.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Soniox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soniox declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Soniox
provider_slug: soniox
scheme_count: 1
schemes:
- evidence: Headers Authorization Required Bearer <SONIOX_API_KEY>
  header: Authorization
  how_to_obtain: Create or retrieve an API key from the Soniox Console (https://console.soniox.com).
  location: header
  name: Bearer
  type: http-bearer
slug: soniox-authentication
source_filename: soniox-authentication.yml
source_heading: Authentication Profile
source_url: https://soniox.com/docs/api-reference/auth/create_temporary_api_key
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://soniox.com/docs/api-reference/auth/create_temporary_api_key\nsources:\n- https://soniox.com/docs/api-reference/auth/create_temporary_api_key\n- https://soniox.com/docs/api-reference/organization/get_organization_project_api_keys\n- https://soniox.com/docs/guides/temporary-api-keys\n- https://soniox.com/docs/guides/websocket-authentication\ndescription: Soniox uses an API key sent as a Bearer token in the Authorization header for both long‑lived and temporary keys.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Headers Authorization Required Bearer <SONIOX_API_KEY>\n  location: header\n  header: Authorization\n  how_to_obtain: Create or retrieve an API key from the Soniox Console (https://console.soniox.com).\nnote: 'Temporary API keys are short‑lived credentials that are also sent using the same Authorization: Bearer header.'\ndocs: https://soniox.com/docs/api-reference/auth/create_temporary_api_key\n"
source_yaml_url: https://artifacts.apis.io/soniox/authentication/soniox-authentication.yml
summary_line: 1 scheme
tags:
- Speech AI
- Multilingual
- Real-time
- Streaming
- API
---
