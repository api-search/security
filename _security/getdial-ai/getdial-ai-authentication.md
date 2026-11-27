---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Dial API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dial declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dial
provider_slug: getdial-ai
scheme_count: 1
schemes:
- evidence: Authenticate every Dial request with a sk_live_ API key sent as a Bearer token.
  header: Authorization
  how_to_obtain: Create an account and key with the CLI (`dial auth login ...`) or via the signup API (`POST /api/v1/auth/signup` then verify).
  location: header
  name: Bearer
  type: http-bearer
slug: getdial-ai-authentication
source_filename: getdial-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.getdial.ai/documentation/get-started/authentication.md
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.getdial.ai/documentation/get-started/authentication.md\nsources:\n- https://docs.getdial.ai/documentation/get-started/authentication.md\n- https://docs.getdial.ai/api-reference/rest-api/authentication/signup.md\n- https://docs.getdial.ai/api-reference/rest-api/authentication/verify-signup.md\n- https://docs.getdial.ai/api-reference/rest-api/authentication/register-number.md\ndescription: Authentication schemes for Dial API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Authenticate every Dial request with a sk_live_ API key sent as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an account and key with the CLI (`dial auth login ...`) or via the signup API (`POST /api/v1/auth/signup` then verify).\nnote: No OAuth2, apiKey, or other schemes are documented.\ndocs: https://docs.getdial.ai/documentation/get-started/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/getdial-ai/authentication/getdial-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Communications
- Telephony
- Messaging
- Voice
---
