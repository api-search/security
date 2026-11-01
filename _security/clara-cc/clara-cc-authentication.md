---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clara-cc-openapi-generated.yml
  format: yaml
  label: Clara API
  slug: clara-cc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clara-cc/openapi/_ae-authored/clara-cc-openapi-generated.yml
auth_types: []
description: 'Clara API uses two-layer authentication: mTLS (mutual TLS) for the connection and OAuth 2.0 Bearer token for each request. Both must be present.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Clara Cc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clara declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Clara
provider_slug: clara-cc
scheme_count: 2
schemes:
- evidence: 'Clara’s API uses two-layer authentication: mTLS (mutual TLS) for the connection and OAuth 2.0 Bearer token for each request.'
  how_to_obtain: Create a project in the Clara dashboard and download the client certificate (public key) and private key.
  name: mutual TLS
  type: mtls
- evidence: 'Each HTTP request must include an Authorization: Bearer <token> header. Tokens are short-lived JWTs obtained from the /oauth/token endpoint using your client_id and client_secret.'
  header: Authorization
  how_to_obtain: Use your client certificate, private key, client_id, and client_secret to POST to the token endpoint (client_credentials flow).
  location: header
  name: OAuth 2.0 Bearer token
  token_url: https://public-api.mx.clara.com/oauth/token
  type: http-bearer
slug: clara-cc-authentication
source_filename: clara-cc-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.clara.team/authentication
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.clara.team/authentication\nsources:\n- https://developers.clara.team/authentication\ndescription: 'Clara API uses two-layer authentication: mTLS (mutual TLS) for the connection and OAuth 2.0 Bearer token for each request. Both\n  must be present.'\nschemes:\n- type: mtls\n  name: mutual TLS\n  evidence: 'Clara’s API uses two-layer authentication: mTLS (mutual TLS) for the connection and OAuth 2.0 Bearer token for each request.'\n  how_to_obtain: Create a project in the Clara dashboard and download the client certificate (public key) and private key.\n- type: http-bearer\n  name: OAuth 2.0 Bearer token\n  evidence: 'Each HTTP request must include an Authorization: Bearer <token> header. Tokens are short-lived JWTs obtained from the /oauth/token\n    endpoint using your client_id and client_secret.'\n  location: header\n  header: Authorization\n  token_url: https://public-api.mx.clara.com/oauth/token\n\
  \  how_to_obtain: Use your client certificate, private key, client_id, and client_secret to POST to the token endpoint (client_credentials flow).\ndocs: https://developers.clara.team/authentication\n"
source_yaml_url: https://artifacts.apis.io/clara-cc/authentication/clara-cc-authentication.yml
summary_line: 2 schemes
tags:
- Fintech
- Spend Management
- Corporate Cards
- Latin America
- AI
---
