---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kamera-ichi-com-auth-api-openapi.yml
  format: yaml
  label: Kamera-ichi 器材市集 Auth API
  slug: kamera-ichi-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kamera-ichi-com/openapi/kamera-ichi-com-auth-api-openapi.yml
- filename: kamera-ichi-com-system-api-openapi.yml
  format: yaml
  label: Kamera-ichi 器材市集 System API
  slug: kamera-ichi-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kamera-ichi-com/openapi/kamera-ichi-com-system-api-openapi.yml
auth_types: []
description: Bearer JWT authentication for member operations
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kamera-ichi 器材市集 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kamera-ichi 器材市集 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kamera-ichi 器材市集
provider_slug: kamera-ichi-com
scheme_count: 1
schemes:
- evidence: 'For authenticated endpoints, provide standard RFC 6750 bearer tokens:'
  header: Authorization
  how_to_obtain: Obtain a JWT by POSTing email and password as JSON to https://kamera-ichi.com/api/auth/token, which returns an access_token with token_type "Bearer".
  location: header
  name: Bearer JWT
  token_url: https://kamera-ichi.com/api/auth/token
  type: http-bearer
slug: kamera-ichi-com-authentication
source_filename: kamera-ichi-com-authentication.yml
source_heading: Authentication Profile
source_url: https://kamera-ichi.com/auth.md
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kamera-ichi.com/auth.md\nsources:\n- https://kamera-ichi.com/auth.md\ndescription: Bearer JWT authentication for member operations\nschemes:\n- type: http-bearer\n  name: Bearer JWT\n  evidence: 'For authenticated endpoints, provide standard RFC 6750 bearer tokens:'\n  location: header\n  header: Authorization\n  token_url: https://kamera-ichi.com/api/auth/token\n  how_to_obtain: Obtain a JWT by POSTing email and password as JSON to https://kamera-ichi.com/api/auth/token, which returns an access_token with\n    token_type \"Bearer\".\ndocs: https://kamera-ichi.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/kamera-ichi-com/authentication/kamera-ichi-com-authentication.yml
summary_line: 1 scheme
tags:
- Marketplace
- Photography
- Secondhand
- Taiwan
---
