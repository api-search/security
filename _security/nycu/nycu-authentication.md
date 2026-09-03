---
api_key_in: []
api_specs:
- filename: nycu-oauth-api-openapi.yml
  format: yaml
  label: NYCU OAuth API
  slug: oauth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nycu/refs/heads/main/openapi/nycu-oauth-api-openapi.yml
auth_types: []
description: How authentication works against the surfaces National Yang Ming Chiao Tung University actually operates. The university runs one first-party authorization server — the NYCU OAuth service at id.nycu.edu.tw, operated by the Information Technology Service Center — and it fronts the university single sign-on account. Everything else NYCU exposes publicly is either anonymous read (OAI-PMH harvesting, the DSpace and Dataverse read APIs) or is gated behind that same SSO.
kind: authentication
layout: security
method: searched
name: Nycu Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Yang Ming Chiao Tung University declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: National Yang Ming Chiao Tung University
provider_slug: nycu
scheme_count: 2
schemes:
- authorization_url: https://id.nycu.edu.tw/o/authorize/
  client_types:
  - public
  - confidential
  evidence:
  - status: 200
    url: https://id.nycu.edu.tw/docs/
  - status: 200
    url: https://id.nycu.edu.tw/policy/
  flow: authorization_code
  grants_not_offered:
  - implicit
  - password
  - client_credentials
  grants_offered:
  - authorization_code
  - refresh_token
  name: NYCU OAuth 2.0 authorization code
  notes: Only the authorization-code grant is offered for user authentication; the terms of service additionally name refresh tokens. Redirect URIs are a per-client whitelist. The terms of service require client implementations to use HTTPS, PKCE and CSRF protection, but PKCE is not enforced or advertised as a server capability in the published documentation.
  registration_url: https://id.nycu.edu.tw/apply/app
  revocation_url: https://id.nycu.edu.tw/o/revoke_token/
  standard: RFC 6749
  surface: https://id.nycu.edu.tw
  token_placement: Authorization Bearer header
  token_url: https://id.nycu.edu.tw/o/token/
  type: oauth2
- evidence:
  - status: 200
    url: https://dataverse.lib.nycu.edu.tw/oai?verb=Identify
  - status: 200
    url: https://ir.lib.nycu.edu.tw/server/oai/request?verb=Identify
  name: Anonymous read
  notes: The OAI-PMH endpoints on both the NYCU Dataverse and the NYCU institutional repository answer unauthenticated GET requests. Verified with verb=Identify.
  surface: https://dataverse.lib.nycu.edu.tw/oai
  type: none
slug: nycu-authentication
source_filename: nycu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: National Yang Ming Chiao Tung University\nproviderId: nycu\ngenerated: '2026-09-01'\nmethod: searched\nsource: https://id.nycu.edu.tw/docs/\nx-operator: institution\ndescription: >-\n  How authentication works against the surfaces National Yang Ming Chiao Tung University\n  actually operates. The university runs one first-party authorization server — the NYCU OAuth\n  service at id.nycu.edu.tw, operated by the Information Technology Service Center — and it\n  fronts the university single sign-on account. Everything else NYCU exposes publicly is either\n  anonymous read (OAI-PMH harvesting, the DSpace and Dataverse read APIs) or is gated behind\n  that same SSO.\nschemes:\n  - name: NYCU OAuth 2.0 authorization code\n    type: oauth2\n    flow: authorization_code\n    standard: RFC 6749\n    surface: https://id.nycu.edu.tw\n    authorization_url: https://id.nycu.edu.tw/o/authorize/\n    token_url:\
  \ https://id.nycu.edu.tw/o/token/\n    revocation_url: https://id.nycu.edu.tw/o/revoke_token/\n    registration_url: https://id.nycu.edu.tw/apply/app\n    token_placement: Authorization Bearer header\n    client_types: [public, confidential]\n    grants_offered: [authorization_code, refresh_token]\n    grants_not_offered: [implicit, password, client_credentials]\n    notes: >-\n      Only the authorization-code grant is offered for user authentication; the terms of service\n      additionally name refresh tokens. Redirect URIs are a per-client whitelist. The terms of\n      service require client implementations to use HTTPS, PKCE and CSRF protection, but PKCE is\n      not enforced or advertised as a server capability in the published documentation.\n    evidence:\n      - url: https://id.nycu.edu.tw/docs/\n        status: 200\n      - url: https://id.nycu.edu.tw/policy/\n        status: 200\n  - name: Anonymous read\n    type: none\n    surface: https://dataverse.lib.nycu.edu.tw/oai\n\
  \    notes: >-\n      The OAI-PMH endpoints on both the NYCU Dataverse and the NYCU institutional repository\n      answer unauthenticated GET requests. Verified with verb=Identify.\n    evidence:\n      - url: https://dataverse.lib.nycu.edu.tw/oai?verb=Identify\n        status: 200\n      - url: https://ir.lib.nycu.edu.tw/server/oai/request?verb=Identify\n        status: 200\ndiscovery:\n  openid_connect: false\n  oauth_authorization_server_metadata: false\n  notes: >-\n    NYCU serves no discovery document. https://id.nycu.edu.tw/.well-known/openid-configuration\n    and https://id.nycu.edu.tw/.well-known/oauth-authorization-server both return 404, probed\n    2026-09-01. This is OAuth 2.0 only, not OpenID Connect. It is the single largest machine\n    -readability gap on the university's own identity surface.\n  evidence:\n    - url: https://id.nycu.edu.tw/.well-known/openid-configuration\n      status: 404\n    - url: https://id.nycu.edu.tw/.well-known/oauth-authorization-server\n\
  \      status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nycu/refs/heads/main/authentication/nycu-authentication.yml
summary_line: 2 schemes
tags:
- Education
- Higher Education
- University
- Taiwan
- Identity
- Authentication
- Single Sign-On
- Research Data
- Institutional Repository
- Library
- Metadata
---
