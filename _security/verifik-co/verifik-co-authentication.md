---
anonymous_access: false
api_key_in: []
api_specs:
- filename: verifik-co-api-openapi.json
  format: json
  label: Verifik AI — x402 KYC & Verifik proxy Api API
  slug: verifik-ai-x402-kyc-verifik-proxy-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verifik-co/openapi/_original/verifik-co-api-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Verifik Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verifik declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Verifik
provider_slug: verifik-co
scheme_count: 1
schemes:
- evidence: Headers  Name Value Authorization <token>
  header: Authorization
  how_to_obtain: Provide a valid JWT token in the Authorization header.
  location: header
  name: Authorization
  type: http-bearer
slug: verifik-co-authentication
source_filename: verifik-co-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.verifik.co/verifik-es/accounts/authentication/renew-your-token-jwt/
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.verifik.co/verifik-es/accounts/authentication/renew-your-token-jwt/\nsources:\n- https://docs.verifik.co/verifik-es/accounts/authentication/renew-your-token-jwt/\n- https://docs.verifik.co/verifik-es/autenticacion/crear-nuevo-token-y-revocar-tokens/\n- https://docs.verifik.co/verifik-es/autenticacion/renovar-tu-token-jwt/\n- https://docs.verifik.co/verifik-es/cuentas/autenticacion/renueva-tu-token-jwt/\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: Headers  Name Value Authorization <token>\n  location: header\n  header: Authorization\n  how_to_obtain: Provide a valid JWT token in the Authorization header.\ndocs: https://docs.verifik.co/verifik-es/accounts/authentication/renew-your-token-jwt/\n"
source_yaml_url: https://artifacts.apis.io/verifik-co/authentication/verifik-co-authentication.yml
summary_line: 1 scheme
tags:
- KYC
- AML
- Facial Recognition
---
