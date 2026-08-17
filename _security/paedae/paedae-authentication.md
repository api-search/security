---
api_key_in: []
api_specs:
- filename: paedae-applications-api-openapi.yml
  format: yaml
  label: Paedae Applications API
  slug: paedae-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-applications-api-openapi.yml
- filename: paedae-beacon-configurations-api-openapi.yml
  format: yaml
  label: Paedae Beacon Configurations API
  slug: paedae-beacon-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-beacon-configurations-api-openapi.yml
- filename: paedae-beacons-api-openapi.yml
  format: yaml
  label: Paedae Beacons API
  slug: paedae-beacons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-beacons-api-openapi.yml
- filename: paedae-communications-api-openapi.yml
  format: yaml
  label: Paedae Communications API
  slug: paedae-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-communications-api-openapi.yml
- filename: paedae-places-api-openapi.yml
  format: yaml
  label: Paedae Places API
  slug: paedae-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-places-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Paedae Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paedae declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Paedae
provider_slug: paedae
scheme_count: 3
schemes:
- applies_to: Manager REST API (applications, places, beacons, beacon configurations, beacon tags, communications)
  description: 'Organization server API key issued in Gimbal Manager under Organizations. Sent verbatim as `Authorization: Token token=<key>` — note the `Token token=` prefix, which is not a standard Bearer scheme.'
  format: Token token=my_organization_server_api_key
  header: Authorization
  id: OrganizationServerApiKey
  in: header
  rotation_documented: false
  type: apiKey
- applies_to: Transmitter / Proximity APIs (/api/v1/transmitters)
  authorization_url: https://manager.gimbal.com/oauth/authorize
  description: The transmitter REST APIs are protected with OAuth and "must have a user token passed as a query parameter" — e.g. `POST /api/v1/transmitters?access_token={token}`. Access is restricted to transmitters owned by the account associated with the token. OAuth also backs the Gimbal Manager portal login (manager.gimbal.com/auth/railsoauth).
  flow: authorizationCode
  id: ProximityOAuth2
  scopes_documented: false
  security_note: Passing a bearer credential in the query string puts it in server logs, proxy logs and Referer headers. This is the provider's documented mechanism, recorded as found.
  token_param: access_token
  token_placement: query
  token_url: https://manager.gimbal.com/oauth/token
  type: oauth2
- applies_to: Infillion Agent Connector (MCP) — NOT the Gimbal REST API
  authorization_url: https://mcp.infillion.com/oauth/authorize
  cross_ref: mcp/paedae-mcp.yml
  description: 'Parent-brand gateway protecting the Infillion Agent Connector MCP endpoint (https://mcp.infillion.com/mcp). An anonymous request returns HTTP 401 with `WWW-Authenticate: Bearer realm="Infillion Gateway"` and an RFC 9728 resource_metadata pointer. Supports dynamic client registration for public clients.'
  flow: authorizationCode
  id: InfillionGatewayOAuth2
  issuer: https://mcp.infillion.com
  pkce: S256
  registration_url: https://mcp.infillion.com/register
  scopes_documented: false
  token_placement: header
  token_url: https://mcp.infillion.com/oauth/token
  type: oauth2
slug: paedae-authentication
source_filename: paedae-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://docs.gimbal.com/rest.html (re-read 2026-08-13); live probe of\n  https://mcp.infillion.com/mcp and its OAuth metadata.\ntype: Authentication\nprovider: Paedae (Gimbal proximity platform, operated by Infillion)\nsummary: >-\n  The Gimbal Manager REST API authenticates with an organization server API key\n  in the Authorization header. The transmitter (beacon) Proximity APIs instead\n  require an OAuth 2.0 user access token passed as a QUERY PARAMETER. The\n  parent's MCP gateway is a separate, spec-compliant OAuth 2.0 protected\n  resource.\nschemes:\n  - id: OrganizationServerApiKey\n    type: apiKey\n    in: header\n    header: Authorization\n    format: 'Token token=my_organization_server_api_key'\n    description: >-\n      Organization server API key issued in Gimbal Manager under Organizations.\n      Sent verbatim as `Authorization: Token token=<key>` — note the\n      `Token token=` prefix, which is not\
  \ a standard Bearer scheme.\n    applies_to: >-\n      Manager REST API (applications, places, beacons, beacon configurations,\n      beacon tags, communications)\n    rotation_documented: false\n  - id: ProximityOAuth2\n    type: oauth2\n    flow: authorizationCode\n    authorization_url: https://manager.gimbal.com/oauth/authorize\n    token_url: https://manager.gimbal.com/oauth/token\n    token_placement: query\n    token_param: access_token\n    description: >-\n      The transmitter REST APIs are protected with OAuth and \"must have a user\n      token passed as a query parameter\" — e.g.\n      `POST /api/v1/transmitters?access_token={token}`. Access is restricted to\n      transmitters owned by the account associated with the token. OAuth also\n      backs the Gimbal Manager portal login\n      (manager.gimbal.com/auth/railsoauth).\n    scopes_documented: false\n    security_note: >-\n      Passing a bearer credential in the query string puts it in server logs,\n      proxy logs\
  \ and Referer headers. This is the provider's documented\n      mechanism, recorded as found.\n    applies_to: Transmitter / Proximity APIs (/api/v1/transmitters)\n  - id: InfillionGatewayOAuth2\n    type: oauth2\n    flow: authorizationCode\n    pkce: S256\n    issuer: https://mcp.infillion.com\n    authorization_url: https://mcp.infillion.com/oauth/authorize\n    token_url: https://mcp.infillion.com/oauth/token\n    registration_url: https://mcp.infillion.com/register\n    token_placement: header\n    description: >-\n      Parent-brand gateway protecting the Infillion Agent Connector MCP\n      endpoint (https://mcp.infillion.com/mcp). An anonymous request returns\n      HTTP 401 with `WWW-Authenticate: Bearer realm=\"Infillion Gateway\"` and an\n      RFC 9728 resource_metadata pointer. Supports dynamic client registration\n      for public clients.\n    scopes_documented: false\n    applies_to: Infillion Agent Connector (MCP) — NOT the Gimbal REST API\n    cross_ref: mcp/paedae-mcp.yml\n\
  content_type: application/json\nunauthorized_status: 401\ndocs: https://docs.gimbal.com/rest.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/authentication/paedae-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Proximity
- Location
- Beacons
- Geofencing
- Mobile SDK
- Advertising
- Marketing
---
