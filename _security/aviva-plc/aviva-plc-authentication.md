---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Aviva Plc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Aviva plc secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Aviva plc
provider_slug: aviva-plc
scheme_count: 2
schemes:
- authorization_endpoint: https://developer.aviva.co.uk/_oauth/authorize
  code_challenge_methods:
  - S256
  evidence: Portal metadata reports oidc_auth_enabled true, rbac_enabled true, basic_auth_enabled false, saml_auth_enabled false, dcr_provider_ids [] — there is no dynamic client registration, so portal accounts are provisioned by Aviva.
  flow: authorizationCode
  grant_types_supported:
  - authorization_code
  issuer: https://developer.aviva.co.uk
  name: portal-login
  oidc_backed: true
  pkce: true
  rbac_enforced: true
  response_types_supported:
  - code
  sources:
  - well-known/aviva-plc-oauth-authorization-server.json
  - https://developer.aviva.co.uk/api/v2/portal
  surface: developer portal (Kong Konnect)
  token_endpoint: https://developer.aviva.co.uk/api/oauth/token
  type: oauth2
- authorization_server: not publicly documented
  bearer: true
  client_credential_fields:
  - Name
  - Client_id
  - Client_secret
  evidence: The developer guide states that for OAuth 2.0 compliant APIs a generated OAuth 2.0 token is supplied in the Authorization field as "Bearer token", and that an authenticated portal user can create, edit or delete an OAuth 2.0 client by entering Name, Client_id and Client_secret — the client credential is then usable for mock testing of the API. Formal production consumption is requested through the Aviva API Gateway.
  flow: clientCredentials
  header: Authorization
  header_format: Bearer <token>
  name: api-consumption
  scopes_published: false
  sources:
  - https://developer.aviva.co.uk/developer-guide
  surface: Aviva API Gateway (business APIs)
  token_endpoint: not publicly documented
  type: oauth2
slug: aviva-plc-authentication
source_filename: aviva-plc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  https://developer.aviva.co.uk/developer-guide (indexed copy — the live page\n  returns HTTP 403 to unauthenticated requests),\n  https://developer.aviva.co.uk/.well-known/oauth-authorization-server (HTTP 200),\n  https://developer.aviva.co.uk/api/v2/portal (HTTP 200)\ndocs: https://developer.aviva.co.uk/developer-guide\nnote: >-\n  Derived from no OpenAPI — Aviva publishes no machine-readable specification.\n  This profile separates the two distinct authentication surfaces Aviva runs: the\n  developer PORTAL login, whose metadata is anonymously readable, and the API\n  CONSUMPTION model, which is described in the portal's developer guide but whose\n  authorization server, scopes and token endpoint are not published outside the\n  login wall.\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials]\n  self_serve: false\n  access_model: partner application and approval\nschemes:\n\
  - name: portal-login\n  surface: developer portal (Kong Konnect)\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  code_challenge_methods: [S256]\n  issuer: https://developer.aviva.co.uk\n  authorization_endpoint: https://developer.aviva.co.uk/_oauth/authorize\n  token_endpoint: https://developer.aviva.co.uk/api/oauth/token\n  grant_types_supported: [authorization_code]\n  response_types_supported: [code]\n  oidc_backed: true\n  rbac_enforced: true\n  sources:\n  - well-known/aviva-plc-oauth-authorization-server.json\n  - https://developer.aviva.co.uk/api/v2/portal\n  evidence: >-\n    Portal metadata reports oidc_auth_enabled true, rbac_enabled true,\n    basic_auth_enabled false, saml_auth_enabled false, dcr_provider_ids [] —\n    there is no dynamic client registration, so portal accounts are provisioned by\n    Aviva.\n- name: api-consumption\n  surface: Aviva API Gateway (business APIs)\n  type: oauth2\n  flow: clientCredentials\n  bearer: true\n  header: Authorization\n\
  \  header_format: Bearer <token>\n  client_credential_fields: [Name, Client_id, Client_secret]\n  authorization_server: not publicly documented\n  token_endpoint: not publicly documented\n  scopes_published: false\n  sources:\n  - https://developer.aviva.co.uk/developer-guide\n  evidence: >-\n    The developer guide states that for OAuth 2.0 compliant APIs a generated\n    OAuth 2.0 token is supplied in the Authorization field as \"Bearer token\", and\n    that an authenticated portal user can create, edit or delete an OAuth 2.0\n    client by entering Name, Client_id and Client_secret — the client credential\n    is then usable for mock testing of the API. Formal production consumption is\n    requested through the Aviva API Gateway.\nnot_documented:\n  api_keys: true\n  mutual_tls: true\n  openid_connect_discovery: true\n  scope_reference: true\n  jwt_claims: true\nonboarding:\n  self_serve_signup: false\n  route: >-\n    Partners discover APIs in the portal catalogue, apply for sandbox\
  \ access, then\n    make a formal request to consume the API through the Aviva API Gateway; access\n    and production consumption are granted by Aviva on approval.\n  contact: aservices@aviva.com\n  contact_page: https://developer.aviva.co.uk/contact\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aviva-plc/refs/heads/main/authentication/aviva-plc-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Insurance
- United Kingdom
- Property and Casualty
- Life Insurance
- Health Insurance
- Claims
- Underwriting
- Brokers
- Workplace Pensions
- Carrier
---
