---
api_key_in: []
api_specs:
- filename: coronet-webhooks-asyncapi.yml
  format: yaml
  label: Coro Public API
  slug: coro-public-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/coronet/refs/heads/main/asyncapi/coronet-webhooks-asyncapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Coronet Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CoroNet secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CoroNet
provider_slug: coronet
scheme_count: 1
schemes:
- credential_source: Coro console > Control Panel > Connectors > API Credentials
  description: To use the Coro API you must first authenticate and obtain a session (bearer) token. Generate a Client ID and Secret credential pair in the Coro console under Control Panel > Connectors > API Credentials (these are not the same as console username/password). POST the credentials to the client authentication endpoint (/oath/token) to receive a bearer token valid for 24 hours.
  flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - docs.coro.net/developer-portal/authentication
  token_endpoint: /oath/token
  token_lifetime: 24h
  type: oauth2
  usage:
    additional_headers:
    - description: The Workspace ID against which the request is executed.
      name: Workspace
    authorization_header: Authentication
slug: coronet-authentication
source_filename: coronet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.coro.net/developer-portal/authentication\ndocs: https://docs.coro.net/developer-portal/authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_type: bearer\n  token_lifetime: 24h\n  request_headers: [Authentication, Workspace]\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  description: >-\n    To use the Coro API you must first authenticate and obtain a session\n    (bearer) token. Generate a Client ID and Secret credential pair in the Coro\n    console under Control Panel > Connectors > API Credentials (these are not\n    the same as console username/password). POST the credentials to the client\n    authentication endpoint (/oath/token) to receive a bearer token valid for\n    24 hours.\n  flow: clientCredentials\n  token_endpoint: /oath/token\n  token_lifetime: 24h\n  credential_source: Coro console > Control Panel > Connectors > API Credentials\n  usage:\n  \
  \  authorization_header: Authentication\n    additional_headers:\n    - name: Workspace\n      description: The Workspace ID against which the request is executed.\n  sources: [docs.coro.net/developer-portal/authentication]\nnotes:\n- Every request sets an Authentication header carrying the bearer token and a\n  Workspace header carrying the target Workspace ID.\n- Token is valid for 24 hours; re-request from /oath/token to refresh.\n- No OpenAPI securityScheme document was retrievable (api.secure.coro.net\n  requires auth); this profile is captured from the published auth docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coronet/refs/heads/main/authentication/coronet-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Enterprise
- Cybersecurity
- Security
- Endpoint Security
- Email Security
- Network Security
- Cloud Security
- Managed Service Providers
- Compliance
- Webhooks
- API
---
