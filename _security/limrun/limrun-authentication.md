---
api_key_in:
- header
api_specs:
- filename: limrun-openapi-original.yml
  format: yaml
  label: Limrun API
  slug: limrun-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limrun/refs/heads/main/openapi/limrun-openapi-original.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Limrun Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Limrun secures its APIs with http, oauth2, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Limrun
provider_slug: limrun
scheme_count: 5
schemes:
- env_var: LIM_API_KEY
  header: Authorization
  in: header
  issued_at: https://console.limrun.com
  key_prefix: lim_
  name: OrgAPIKey
  scheme: bearer
  scope: The REST control plane at api.limrun.com - create, list, get, and delete instances and assets.
  source: docs
  type: http
  warning: Must never ship to a browser or end-user client.
- header: Authorization
  in: header
  name: PerInstanceToken
  obtained_from: instance.status.token (returned when the instance reaches ready)
  scheme: bearer
  scope: The per-instance data plane - apiUrl device daemon, endpointWebSocketUrl (also accepted as a ?token= query parameter), adbWebSocketUrl, sandbox.xcode.url, and the per-instance MCP endpoint. Embedded in signedStreamUrl for browser streaming. Valid only while the instance runs and only for that instance.
  source: docs
  type: http
- name: SignedStreamURL
  obtained_from: instance.status.signedStreamUrl
  scope: Browser watch URL with the token baked in. Anyone holding the URL can open the running simulator without an interactive auth flow - the mechanism for sharing a live device with a reviewer.
  source: docs
  type: bearer-in-url
- flows:
  - authorizationUrl: https://api.limrun.com/authn/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    issuer: https://api.limrun.com
    registrationUrl: https://api.limrun.com/authn/oauth/register
    scopes:
    - mcp
    tokenUrl: https://api.limrun.com/authn/oauth/token
    token_endpoint_auth_methods:
    - none
  name: MCPOAuth
  source: https://api.limrun.com/.well-known/oauth-authorization-server
  type: oauth2
- docs: https://docs.limrun.com/docs/reference/single-sign-on
  name: OrganizationSSO
  scope: Organization single sign-on for the Limrun console; Okta Integration Network supported.
  source: docs
  type: openIdConnect
slug: limrun-authentication
source_filename: limrun-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/limrun-openapi-original.yml\ndocs: https://docs.limrun.com/docs/reference/sdk\nnotes: >-\n  The harvested OpenAPI declares no components.securitySchemes, so the mechanical derive produced\n  nothing. This profile is taken from the provider's SDK reference, MCP page, and the live RFC 8414\n  document at api.limrun.com. Limrun uses two distinct credentials plus an OAuth surface reserved\n  for MCP, and separately offers OIDC single sign-on for console access.\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OrgAPIKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  key_prefix: lim_\n  env_var: LIM_API_KEY\n  issued_at: https://console.limrun.com\n  scope: >-\n    The REST control plane at api.limrun.com - create, list, get, and delete instances and assets.\n  warning: Must never ship to a browser\
  \ or end-user client.\n  source: docs\n- name: PerInstanceToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  obtained_from: instance.status.token (returned when the instance reaches ready)\n  scope: >-\n    The per-instance data plane - apiUrl device daemon, endpointWebSocketUrl (also accepted as a\n    ?token= query parameter), adbWebSocketUrl, sandbox.xcode.url, and the per-instance MCP endpoint.\n    Embedded in signedStreamUrl for browser streaming. Valid only while the instance runs and only\n    for that instance.\n  source: docs\n- name: SignedStreamURL\n  type: bearer-in-url\n  obtained_from: instance.status.signedStreamUrl\n  scope: >-\n    Browser watch URL with the token baked in. Anyone holding the URL can open the running simulator\n    without an interactive auth flow - the mechanism for sharing a live device with a reviewer.\n  source: docs\n- name: MCPOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    issuer: https://api.limrun.com\n\
  \    authorizationUrl: https://api.limrun.com/authn/oauth/authorize\n    tokenUrl: https://api.limrun.com/authn/oauth/token\n    registrationUrl: https://api.limrun.com/authn/oauth/register\n    code_challenge_methods:\n    - S256\n    token_endpoint_auth_methods:\n    - none\n    scopes:\n    - mcp\n  source: https://api.limrun.com/.well-known/oauth-authorization-server\n- name: OrganizationSSO\n  type: openIdConnect\n  scope: Organization single sign-on for the Limrun console; Okta Integration Network supported.\n  docs: https://docs.limrun.com/docs/reference/single-sign-on\n  source: docs\ncredential_confusion_note: >-\n  The provider's own SDK reference calls out mixing the org API key and the per-instance token as\n  \"the most common integration bug\". The two pages also disagree on which credential authenticates\n  MCP - see mcp/limrun-mcp.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/limrun/refs/heads/main/authentication/limrun-authentication.yml
summary_line: http/oauth2/openIdConnect · 5 schemes
tags:
- Company
- Mobile
- iOS
- Android
- Simulators
- Emulators
- Cloud Infrastructure
- Continuous Integration
- Developer Tools
- Testing
- Agents
- Model Context Protocol
- Sandboxes
- Xcode
---
