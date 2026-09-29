---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bitpagos-openapi-generated.yml
  format: yaml
  label: Bitpagos API
  slug: bitpagos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpagos/refs/heads/main/openapi/_ae-authored/bitpagos-openapi-generated.yml
auth_types: []
description: Authentication methods for Bitpagos (Ripio) services
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Bitpagos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitpagos declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Bitpagos
provider_slug: bitpagos
scheme_count: 4
schemes:
- evidence: Your server calls `POST /auth` and receives a `session_code`.
  how_to_obtain: Send a POST request to https://b2b-crypto-widget-api.sandbox.ripio.com/api/v1/auth with JSON body containing `client_id`, `client_secret` and `external_ref`.
  location: body
  name: Session code request
  type: other
- evidence: This service provides an access JWT token for the user to use the On Ramp Widget.
  how_to_obtain: POST to https://b2b-widget-onramp-api.ripio.com/api/v1/auth (or sandbox URL) with form‑urlencoded fields `username` (client_id:external_ref[:address]) and `password` (client_secret).
  location: body
  name: On‑Ramp widget token request
  type: other
- evidence: Every call to the API has to be authenticated with an OAuth2 Token.
  how_to_obtain: Send a POST request to the token endpoint with Basic Authorization header (Base64‑encoded `client_id:client_secret`) and form field `grant_type=client_credentials`.
  name: Ramp API OAuth2 client credentials
  token_url: https://skala-sandbox.ripio.com/oauth2/token/
  type: oauth2
- evidence: Header Description Authorization The API key as a string.
  header: Authorization
  how_to_obtain: Create API credentials in the Ripio portal to obtain an API Token, then include it in the `Authorization` header of private requests.
  location: header
  name: API Token header
  type: apiKey
slug: bitpagos-authentication
source_filename: bitpagos-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ripio.com/crypto-as-a-service/widget/get-started/authentication.md
source_yaml: "generated: '2026-09-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ripio.com/crypto-as-a-service/widget/get-started/authentication.md\nsources:\n- https://docs.ripio.com/crypto-as-a-service/widget/get-started/authentication.md\n- https://docs.ripio.com/ramps-api/widget/get-started/authentication.md\n- https://docs.ripio.com/ramps-api/authentication/acquire-access-token.md\n- https://apidocs.ripio.com/static/api/authentication\ndescription: Authentication methods for Bitpagos (Ripio) services\nschemes:\n- type: other\n  name: Session code request\n  evidence: Your server calls `POST /auth` and receives a `session_code`.\n  location: body\n  how_to_obtain: Send a POST request to https://b2b-crypto-widget-api.sandbox.ripio.com/api/v1/auth with JSON body containing `client_id`, `client_secret`\n    and `external_ref`.\n- type: other\n  name: On‑Ramp widget token request\n  evidence: This service provides an access JWT token for the user\
  \ to use the On Ramp Widget.\n  location: body\n  how_to_obtain: POST to https://b2b-widget-onramp-api.ripio.com/api/v1/auth (or sandbox URL) with form‑urlencoded fields `username` (client_id:external_ref[:address])\n    and `password` (client_secret).\n- type: oauth2\n  name: Ramp API OAuth2 client credentials\n  evidence: Every call to the API has to be authenticated with an OAuth2 Token.\n  token_url: https://skala-sandbox.ripio.com/oauth2/token/\n  how_to_obtain: Send a POST request to the token endpoint with Basic Authorization header (Base64‑encoded `client_id:client_secret`) and form\n    field `grant_type=client_credentials`.\n- type: apiKey\n  name: API Token header\n  evidence: Header Description Authorization The API key as a string.\n  location: header\n  header: Authorization\n  how_to_obtain: Create API credentials in the Ripio portal to obtain an API Token, then include it in the `Authorization` header of private requests.\ndocs: https://docs.ripio.com/crypto-as-a-service/widget/get-started/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitpagos/refs/heads/main/authentication/bitpagos-authentication.yml
summary_line: 4 schemes
tags:
- Payments
- Fintech
- Latin America
- Bitcoin
- CreditCards
---
