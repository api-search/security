---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clara-com-mx-openapi-generated.yml
  format: yaml
  label: Clara API
  slug: clara-com-mx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clara-com-mx/openapi/_ae-authored/clara-com-mx-openapi-generated.yml
auth_types: []
description: 'Clara’s API uses two-layer authentication: mTLS (mutual TLS) for the connection and OAuth 2.0 Bearer token for each request. Both must be present — a valid token without a client certificate will be rejected, and vice versa.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Clara Com Mx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clara declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Clara
provider_slug: clara-com-mx
scheme_count: 2
schemes:
- evidence: 'Certificate layer (mTLS): Your client certificate authenticates the connection at the TLS level.'
  how_to_obtain: Download your client certificate and private key when creating a project in the Clara dashboard.
  name: mTLS
  type: mtls
- evidence: 'Each HTTP request must include an Authorization: Bearer <token> header.'
  header: Authorization
  how_to_obtain: Use your client certificate, private key, client_id, and client_secret to request a token via the /oauth/token endpoint (client_credentials flow).
  location: header
  name: OAuth 2.0 Bearer token
  token_url: https://public-api.mx.clara.com/oauth/token
  type: http-bearer
slug: clara-com-mx-authentication
source_filename: clara-com-mx-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.clara.team/authentication
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.clara.team/authentication\nsources:\n- https://developers.clara.team/authentication\ndescription: 'Clara’s API uses two-layer authentication: mTLS (mutual TLS) for the connection and OAuth 2.0 Bearer token for each request. Both\n  must be present — a valid token without a client certificate will be rejected, and vice versa.'\nschemes:\n- type: mtls\n  name: mTLS\n  evidence: 'Certificate layer (mTLS): Your client certificate authenticates the connection at the TLS level.'\n  how_to_obtain: Download your client certificate and private key when creating a project in the Clara dashboard.\n- type: http-bearer\n  name: OAuth 2.0 Bearer token\n  evidence: 'Each HTTP request must include an Authorization: Bearer <token> header.'\n  location: header\n  header: Authorization\n  token_url: https://public-api.mx.clara.com/oauth/token\n  how_to_obtain: Use your client certificate,\
  \ private key, client_id, and client_secret to request a token via the /oauth/token endpoint (client_credentials\n    flow).\ndocs: https://developers.clara.team/authentication\n"
source_yaml_url: https://artifacts.apis.io/clara-com-mx/authentication/clara-com-mx-authentication.yml
summary_line: 2 schemes
tags:
- Corporate Cards
- Expense Management
- Accounts Payable
- Travel Pay
- AI Finance
- Latin America
- ERP Integration
---
