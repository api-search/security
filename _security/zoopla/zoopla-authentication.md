---
api_key_in: []
api_specs:
- filename: zoopla-products-api-openapi.yml
  format: yaml
  label: Zoopla Products API
  slug: zoopla-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoopla/refs/heads/main/openapi/zoopla-products-api-openapi.yml
- filename: zoopla-rest-endpoints-api-openapi.yml
  format: yaml
  label: Zoopla REST Endpoints API
  slug: zoopla-rest-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoopla/refs/heads/main/openapi/zoopla-rest-endpoints-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zoopla Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Zoopla secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Zoopla
provider_slug: zoopla
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token
  name: OAuth2
  sources:
  - openapi/zoopla-leads-api-openapi.json
  - openapi/zoopla-premium-listing-activations-openapi.json
  - openapi/zoopla-weekly-featured-property-activations-openapi.json
  type: oauth2
slug: zoopla-authentication
source_filename: zoopla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\ndocs: https://developers.zoopla.co.uk/pages/authentication\nsource: openapi/zoopla-leads-api-openapi.json, openapi/zoopla-premium-listing-activations-openapi.json,\n  openapi/zoopla-weekly-featured-property-activations-openapi.json, https://developers.zoopla.co.uk/pages/authentication,\n  https://developers.zoopla.co.uk/leads/docs/push-service\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  self_serve: false\n  identity_provider: Amazon Cognito (eu-west-1)\n  api_request_header: 'Authorization: Bearer {access_token}'\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/zoopla-leads-api-openapi.json\n  - openapi/zoopla-premium-listing-activations-openapi.json\n  - openapi/zoopla-weekly-featured-property-activations-openapi.json\ntoken_request:\n  method: POST\n  url: https://services-auth.services.zoopla.co.uk/oauth2/token\n\
  \  client_authentication: >-\n    HTTP Basic — Authorization: Basic base64(client_id:client_secret). The Leads\n    documentation also shows the credentials form-encoded in the body with an\n    `audience` parameter set to the integration URL (https://services.zoopla.co.uk),\n    and notes the fields are form-encoded rather than sent as a JSON body.\n  content_type: application/x-www-form-urlencoded\n  grant_type: client_credentials\n  scope_parameter: scope=api/api_access (activation APIs)\n  response:\n    token_type: Bearer\n    expires_in: 3600\n  issuer: https://cognito-idp.eu-west-1.amazonaws.com/eu-west-1_g0qeZRnbT\n  issuer_evidence: >-\n    The sample access token published on the authentication page decodes to an\n    `iss` claim naming that Cognito user pool, which places the auth tier in AWS\n    eu-west-1.\ncredential_issuance:\n  self_serve: false\n  process: >-\n    Generate a 4096-bit RSA GPG key pair, export the public key and give it to\n    your Zoopla technical contact.\
  \ Zoopla returns a plaintext client_id and a\n    PGP-encrypted client_secret which you decrypt with your private key.\n  prerequisite: >-\n    You must already be a Zoopla customer subscribed to a listings package with\n    the relevant features.\n  contact: members@zoopla.co.uk\n  revocation: >-\n    Contact your technical contact immediately to revoke a compromised\n    client_id/client_secret pair and be issued a new one.\nerrors:\n  invalid_or_expired_token:\n  - 401\n  - 403\ntoken_handling:\n  caching: >-\n    Cache the access token for its full expires_in window. The Leads docs name\n    per-request token minting as the cause of HTTP 429 \"service busy\" responses.\ninbound_authentication:\n  context: Lead Push Service — Zoopla is the client, the member is the server.\n  methods:\n  - method: oauth2\n    grant: client_credentials\n    note: >-\n      The member supplies client_id, client_secret, a token endpoint and\n      (configuration dependent) an audience. Zoopla mints a token\
  \ and sends\n      'Authorization: Bearer {access_token}'.\n  - method: api_key\n    note: >-\n      The member supplies a key; Zoopla sends it verbatim as the Authorization\n      header value with no scheme prefix.\n  signature_verification: none\n  docs: https://developers.zoopla.co.uk/leads/docs/push-service\ndiscovery:\n  openid_configuration: 404\n  oauth_authorization_server: 404\n  note: >-\n    Neither the API host nor the Cognito-fronted token host serves OIDC discovery\n    or RFC 8414 authorization-server metadata; the OAuth setup is documented in\n    prose only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoopla/refs/heads/main/authentication/zoopla-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Real-Estate
- United Kingdom
- Property Listings
- Property Portal
- PropTech
- Rentals
- Estate Agents
- Leads
- CRM Integration
---
