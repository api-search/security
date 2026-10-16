---
anonymous_access: false
api_key_in: []
api_specs:
- filename: curios-openapi-generated.yml
  format: yaml
  label: Curios API
  slug: curios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curios/refs/heads/main/openapi/_ae-authored/curios-openapi-generated.yml
auth_types: []
description: Authentication methods for Curios APIs
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Curios Authentication
name_suffix: Authentication
oauth_flows: []
overview: Curios declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Curios
provider_slug: curios
scheme_count: 3
schemes:
- evidence: '-H '' curios-api-key: {API Key} '''
  header: curios-api-key
  location: header
  name: curios-api-key
  type: apiKey
- evidence: Authorization Bearer {JWT} The JWT session token issued upon succesful customer login and verification.
  header: Authorization
  how_to_obtain: Use customers/login and customers/verify endpoints to retrieve a JSON Web Token (JWT).
  location: header
  name: Bearer JWT
  type: http-bearer
- evidence: Every request must include a signature in the curios-signature header value.
  header: curios-signature
  how_to_obtain: Create signature using HMAC SHA256 with your API Secret as the encryption key.
  location: header
  name: curios-signature
  type: hmac
slug: curios-authentication
source_filename: curios-authentication.yml
source_heading: Authentication Profile
source_url: https://content.curios.com/docs/admin-tokens
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://content.curios.com/docs/admin-tokens\nsources:\n- https://content.curios.com/docs/admin-tokens\n- https://content.curios.com/docs/casper\n- https://content.curios.com/docs/\n- https://content.curios.com/docs/admin\ndescription: Authentication methods for Curios APIs\nschemes:\n- type: apiKey\n  name: curios-api-key\n  evidence: '-H '' curios-api-key: {API Key} '''\n  location: header\n  header: curios-api-key\n- type: http-bearer\n  name: Bearer JWT\n  evidence: Authorization Bearer {JWT} The JWT session token issued upon succesful customer login and verification.\n  location: header\n  header: Authorization\n  how_to_obtain: Use customers/login and customers/verify endpoints to retrieve a JSON Web Token (JWT).\n- type: hmac\n  name: curios-signature\n  evidence: Every request must include a signature in the curios-signature header value.\n  location: header\n  header: curios-signature\n\
  \  how_to_obtain: Create signature using HMAC SHA256 with your API Secret as the encryption key.\ndocs: https://content.curios.com/docs/admin-tokens\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curios/refs/heads/main/authentication/curios-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Marketplace
- Web3
- API
- Creator
---
