---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for the FOTOhub API as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: FOTOhub Authentication
name_suffix: Authentication
oauth_flows: []
overview: FOTOhub declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FOTOhub
provider_slug: fotohub-app
scheme_count: 2
schemes:
- evidence: Pass your API key in the Authorization header using the Bearer scheme.
  header: Authorization
  how_to_obtain: Create a key in the FOTOhub console (Console → API Keys) or programmatically via POST /v1/auth/keys (requires a session JWT). The key format is fh_live_ followed by 32 lowercase hex characters (40 characters total).
  location: header
  name: API Key Bearer Token
  type: http-bearer
- evidence: 'all authenticate with your session JWT ( Authorization: Bearer <session_jwt> , the same token the console uses)'
  header: Authorization
  how_to_obtain: Obtain a session JWT by logging into the FOTOhub web console; the JWT is used for key‑management endpoints (POST /v1/auth/keys, PATCH /v1/auth/keys/{key_id}, DELETE /v1/auth/keys/{key_id}, etc.).
  location: header
  name: Session JWT
  type: http-bearer
slug: fotohub-app-authentication
source_filename: fotohub-app-authentication.yml
source_heading: Authentication Profile
source_url: https://fotohub.app/fh/guide/api-keys
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fotohub.app/fh/guide/api-keys\nsources:\n- https://fotohub.app/fh/guide/api-keys\n- https://docs.fotohub.app/api/authentication\n- https://fotohub.app/fh/guide/getting-started\n- https://fotohub.app/fh/guide/public-api-quickstart\ndescription: Authentication methods for the FOTOhub API as documented.\nschemes:\n- type: http-bearer\n  name: API Key Bearer Token\n  evidence: Pass your API key in the Authorization header using the Bearer scheme.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the FOTOhub console (Console → API Keys) or programmatically via POST /v1/auth/keys (requires a session JWT).\n    The key format is fh_live_ followed by 32 lowercase hex characters (40 characters total).\n- type: http-bearer\n  name: Session JWT\n  evidence: 'all authenticate with your session JWT ( Authorization: Bearer <session_jwt> , the same token the\
  \ console uses)'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a session JWT by logging into the FOTOhub web console; the JWT is used for key‑management endpoints (POST /v1/auth/keys,\n    PATCH /v1/auth/keys/{key_id}, DELETE /v1/auth/keys/{key_id}, etc.).\ndocs: https://fotohub.app/fh/guide/api-keys\n"
source_yaml_url: https://artifacts.apis.io/fotohub-app/authentication/fotohub-app-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Multimedia
- Image Generation
- Video Generation
- Audio Generation
- 3D
- Platform
---
