---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pinch-openapi-generated.yml
  format: yaml
  label: Pinch API
  slug: pinch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch/refs/heads/main/openapi/_ae-authored/pinch-openapi-generated.yml
auth_types: []
description: Pinch API authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Pinch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pinch declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Pinch
provider_slug: pinch
scheme_count: 2
schemes:
- evidence: The Pinch API uses **OAuth 2.0 client credentials** for authentication. Every API request requires a Bearer token, which you obtain by exchanging your **Application ID** and **Secret Key**.
  flows:
  - client_credentials
  how_to_obtain: Make a POST request to the token endpoint with your Application ID and Secret Key using HTTP Basic Auth or by including `client_id` and `client_secret` in the form‑encoded body.
  name: OAuth 2.0 client credentials
  scopes:
  - api1
  token_url: https://auth.getpinch.com.au/connect/token
  type: oauth2
- evidence: 'Include the token in the `Authorization` header of every API request:'
  header: Authorization
  how_to_obtain: Obtain the token via the OAuth 2.0 client credentials flow described above.
  location: header
  name: Bearer token
  type: http-bearer
slug: pinch-authentication
source_filename: pinch-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.getpinch.com.au/docs/application-authentication.md
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.getpinch.com.au/docs/application-authentication.md\nsources:\n- https://docs.getpinch.com.au/docs/application-authentication.md\n- https://docs.getpinch.com.au/reference/tokens.md\n- https://docs.getpinch.com.au/reference/tokens\n- https://docs.getpinch.com.au/docs/application-authentication\ndescription: Pinch API authentication\nschemes:\n- type: oauth2\n  name: OAuth 2.0 client credentials\n  evidence: The Pinch API uses **OAuth 2.0 client credentials** for authentication. Every API request requires a Bearer token, which you obtain\n    by exchanging your **Application ID** and **Secret Key**.\n  flows:\n  - client_credentials\n  token_url: https://auth.getpinch.com.au/connect/token\n  scopes:\n  - api1\n  how_to_obtain: Make a POST request to the token endpoint with your Application ID and Secret Key using HTTP Basic Auth or by including `client_id`\n    and `client_secret`\
  \ in the form‑encoded body.\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Include the token in the `Authorization` header of every API request:'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain the token via the OAuth 2.0 client credentials flow described above.\ndocs: https://docs.getpinch.com.au/docs/application-authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinch/refs/heads/main/authentication/pinch-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Payments
- MedicalSpa
- API
- HealthTech
---
