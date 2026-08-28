---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Muck Rack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Muck Rack declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Muck Rack
provider_slug: muck-rack
scheme_count: 1
schemes:
- evidence:
    no_credential:
      body: '{"detail":"Authentication credentials were not provided."}'
      request: GET /api/saved-searches/ with no Authorization header
      status: 403
    wrong_credential_bearer:
      body: '{"detail":"Invalid API key"}'
      interpretation: The message changes from "credentials were not provided" to "Invalid API key", proving the server parsed the Bearer credential and rejected its value. This is the authoritative signal for the scheme.
      request: 'GET /api/saved-searches/ with Authorization: Bearer <invalid>'
      status: 403
    wrong_credential_token:
      body: '{"detail":"Authentication credentials were not provided."}'
      interpretation: DRF TokenAuthentication is NOT enabled; the header was ignored.
      request: 'GET /api/saved-searches/ with Authorization: Token <invalid>'
      status: 403
    wrong_credential_x_api_key:
      body: '{"detail":"Authentication credentials were not provided."}'
      interpretation: No custom API-key header is honoured.
      request: 'GET /api/saved-searches/ with X-API-Key: <invalid>'
      status: 403
  format: 'Authorization: Bearer <api key>'
  header: Authorization
  in: header
  name: apiKeyBearer
  scheme: bearer
  type: http
slug: muck-rack-authentication
source_filename: muck-rack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  Live unauthenticated probes of https://muckrack.com/api/saved-searches/ (2026-08-26),\n  corroborated by https://help.muckrack.com/en/articles/10175260-muck-rack-api and\n  https://muckrack.com/pr-software/api\ndocs: https://help.muckrack.com/en/articles/10175260-muck-rack-api\nnote: >-\n  Derived from live response behaviour, not from a specification — Muck Rack publishes\n  no OpenAPI and its API reference is visible only to authenticated customers. The\n  scheme below was established by differential probing: sending no credential and\n  sending a syntactically-valid-but-wrong credential in each of three header styles,\n  and reading which error the origin returned. Only the HTTP Bearer style produced a\n  key-specific rejection, which identifies it as the credential the server actually\n  parses.\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization:\
  \ Bearer <api key>'\n  evidence:\n    no_credential:\n      request: GET /api/saved-searches/ with no Authorization header\n      status: 403\n      body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n    wrong_credential_bearer:\n      request: 'GET /api/saved-searches/ with Authorization: Bearer <invalid>'\n      status: 403\n      body: '{\"detail\":\"Invalid API key\"}'\n      interpretation: >-\n        The message changes from \"credentials were not provided\" to \"Invalid API key\",\n        proving the server parsed the Bearer credential and rejected its value. This is\n        the authoritative signal for the scheme.\n    wrong_credential_token:\n      request: 'GET /api/saved-searches/ with Authorization: Token <invalid>'\n      status: 403\n      body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n      interpretation: DRF TokenAuthentication is NOT enabled; the header was ignored.\n    wrong_credential_x_api_key:\n      request: 'GET\
  \ /api/saved-searches/ with X-API-Key: <invalid>'\n      status: 403\n      body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n      interpretation: No custom API-key header is honoured.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes:\n  model: none\n  note: >-\n    No OAuth surface exists, so there is no scope model. Authorization is\n    organization-wide and coarse-grained: one key represents the organization and\n    reaches the Saved Searches its account owns. scopes/ is deliberately not emitted.\nkey_management:\n  issuer: Account Admin\n  location: Muck Rack web app -> Organization Settings -> API Keys\n  self_service: false\n  note: >-\n    Keys can only be created once the API add-on has been purchased; an Admin user\n    presses \"+ Create New\" and supplies a description. There is no public developer\n    signup that yields a key.\n  rotation: not documented publicly\n  expiry: not documented publicly\nentitlement:\n  required_plan: Premier\n\
  \  add_on: true\n  note: The API is a paid add-on to the Premier tier, not included in any published plan.\ngaps:\n- No public OpenAPI or auth reference; the scheme above is inferred from live behaviour\n  rather than read from a contract.\n- Key rotation, expiry and revocation semantics are not documented publicly.\n- No scoped or least-privilege credential is offered; one organization key is all-or-nothing.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/muck-rack/refs/heads/main/authentication/muck-rack-authentication.yml
summary_line: 1 scheme
tags:
- Public Relations
- Media Monitoring
- Media Database
- Journalists
- Communications
- Press Releases
- Earned Media
- Social Listening
- Marketing
- News
- Analytics
- Company
---
