---
api_key_in: []
api_specs:
- filename: schema
  format: yaml
  label: Jamf Pro API
  slug: jamf-pro-api
  spec_type: OpenAPI
  url: https://your-instance.jamfcloud.com/api/schema
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Jamf Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: JAMF secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: JAMF
provider_slug: jamf
scheme_count: 3
schemes:
- description: 'Request a token with POST /api/v1/auth/token using basic auth (user account + password). The response returns a token and expiration; send it as `Authorization: Bearer <token>`. Tokens expire after ~20 minutes and can be renewed with POST /api/v1/auth/keep-alive. Invalidate with POST /api/v1/auth/invalidate-token.'
  keep_alive_url: /api/v1/auth/keep-alive
  name: BearerToken
  scheme: bearer
  token_url: /api/v1/auth/token
  ttl_minutes: 20
  type: http
- authorization_model: api-roles
  description: Since Jamf Pro 10.49.0. Create an API Client (client id + secret) and assign it one or more API Roles. Exchange the client id/secret for an access token scoped exclusively to Jamf Pro APIs, protecting admin UI credentials. Adding/removing an API Role requires client-secret rotation to take effect; adding/removing a privilege on a role takes effect for new tokens immediately.
  flow: clientCredentials
  name: ClientCredentials
  type: oauth2
- description: Used to obtain a bearer token (Classic API historically accepted basic auth directly; bearer tokens are now the recommended path for both the Jamf Pro API and the Classic API).
  name: BasicAuth
  scheme: basic
  type: http
slug: jamf-authentication
source_filename: jamf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.jamf.com/jamf-pro/docs/client-credentials\ndocs:\n- https://developer.jamf.com/jamf-pro/docs/jamf-pro-api-overview\n- https://developer.jamf.com/jamf-pro/docs/client-credentials\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer, basic]\n  oauth2_flows: [clientCredentials]\n  model: >-\n    Jamf Pro uses short-lived bearer tokens. Tokens are obtained either from\n    user credentials (basic auth) or, since Jamf Pro 10.49.0, from OAuth\n    client-credential API Clients. Authorization is governed by API Roles\n    (collections of privileges) rather than OAuth scopes.\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    Request a token with POST /api/v1/auth/token using basic auth (user\n    account + password). The response returns a token and expiration; send it\n    as `Authorization: Bearer <token>`. Tokens expire after ~20 minutes and\n    can be renewed with POST\
  \ /api/v1/auth/keep-alive. Invalidate with\n    POST /api/v1/auth/invalidate-token.\n  token_url: /api/v1/auth/token\n  keep_alive_url: /api/v1/auth/keep-alive\n  ttl_minutes: 20\n- name: ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Since Jamf Pro 10.49.0. Create an API Client (client id + secret) and\n    assign it one or more API Roles. Exchange the client id/secret for an\n    access token scoped exclusively to Jamf Pro APIs, protecting admin UI\n    credentials. Adding/removing an API Role requires client-secret rotation\n    to take effect; adding/removing a privilege on a role takes effect for\n    new tokens immediately.\n  authorization_model: api-roles\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: >-\n    Used to obtain a bearer token (Classic API historically accepted basic\n    auth directly; bearer tokens are now the recommended path for both the\n    Jamf Pro API and the Classic API).\nauthorization:\n  model: API\
  \ Roles and Clients\n  concept: >-\n    An API Role is a collection of privileges defining which endpoints an API\n    Client can access. Multiple roles can be assigned to one client for\n    cumulative privileges. Managed via the api-roles, api-integrations, and\n    api-role-privileges endpoints, or the Jamf Pro UI.\n  privilege_lookup: /api/v1/api-role-privileges\nnotes: >-\n  Jamf uses privileges via API Roles rather than OAuth scopes, so no OAuth\n  scope reference (scopes/) artifact is emitted; authentication carries the\n  authorization model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jamf/refs/heads/main/authentication/jamf-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Apple Device Management
- MDM
- Endpoint Security
- Mobile Device Management
- IT Operations
- Identity
- Compliance
- Developer Tools
- Enterprise
---
