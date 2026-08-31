---
api_key_in: []
api_specs:
- filename: meero-asynchronous-api-openapi.yml
  format: yaml
  label: Meero Asynchronous API
  slug: meero-asynchronous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/openapi/meero-asynchronous-api-openapi.yml
- filename: meero-feature-api-openapi.yml
  format: yaml
  label: Meero Feature API
  slug: meero-feature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/openapi/meero-feature-api-openapi.yml
- filename: meero-synchronous-api-openapi.yml
  format: yaml
  label: Meero Synchronous API
  slug: meero-synchronous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/openapi/meero-synchronous-api-openapi.yml
- filename: meero-vehicle-api-openapi.yml
  format: yaml
  label: Meero Vehicle API
  slug: meero-vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/openapi/meero-vehicle-api-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Meero Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meero secures its APIs with http, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Meero
provider_slug: meero
scheme_count: 4
schemes:
- applied: root-level security on every operation
  detail: The scheme is named "api_key" but declared as HTTP bearer. Tokens are issued per CarCutter account; there are no scopes, no token endpoint and no documented rotation or expiry policy. The 401 message the contract publishes is "submitted 'Bearer' token is unauthorized".
  name: api_key
  observed:
    body_content_type: text/html
    http_status: 401
    note: The live 401 body is an HTML "401 Unauthorized" page, not the JSON UnauthorizedResponse the contract documents — a real gap between contract and runtime.
    request: GET https://api.car-cutter.com/vehicle/status?vehicle_id=test (no Authorization header)
  scheme: bearer
  sources:
  - openapi/meero-carcutter-openapi.json
  surface: public REST API (https://api.car-cutter.com)
  type: http
- detail: A keyless demo composition path documented in github.com/carcutter/carcutter-api-samples. Probed unauthenticated on 2026-08-25 and returned 400 "invalid file" rather than 401, confirming it requires no credential. See sandbox/meero-sandbox.yml.
  name: none (public demo)
  surface: POST https://api.car-cutter.com/vehicle/composition/segment
  type: none
- client_registration: client_id_metadata_document (no client secret)
  detail: RFC 8414 + RFC 9728 compliant; the MCP 401 returns a WWW-Authenticate header pointing at the protected-resource metadata.
  discovery:
  - https://www.carcutter.com/.well-known/oauth-authorization-server
  - https://www.carcutter.com/.well-known/oauth-protected-resource
  flows:
    authorizationCode:
      authorizationUrl: https://www.carcutter.com/oauth/authorize
      refreshUrl: https://www.carcutter.com/oauth/token
      scopes:
        mcp: Access to the CarCutter MCP server resource.
      tokenUrl: https://www.carcutter.com/oauth/token
  name: carcutter_mcp_oauth
  pkce: S256
  surface: https://www.carcutter.com/wp-json/mcp/mcp-oauth-server
  type: oauth2
- detail: Discovered from the Hub login redirect. api2.car-cutter.com is an AWS API Gateway that answers every path with 403 {"message":"Missing Authentication Token"} — there is no public contract for it, so it is recorded but not profiled.
  name: carcutter_hub_oidc
  openIdConnectUrl: https://auth.eu.car-cutter.com/.well-known/openid-configuration
  pkce:
  - S256
  - plain
  provider: Auth0
  scopes_requested_by_hub:
  - openid
  - offline_access
  surface: CarCutter Hub (https://hub.car-cutter.com/) and the gated audience https://api2.car-cutter.com
  type: openIdConnect
slug: meero-authentication
source_filename: meero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: openapi/meero-carcutter-openapi.json + live probes of api.car-cutter.com, hub.car-cutter.com, auth.eu.car-cutter.com and www.carcutter.com on 2026-08-25\ndocs: https://cloud.car-cutter.com/doc/api.html\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  note: 'Three distinct authentication surfaces, only one of which is the public product API.'\nschemes:\n- name: api_key\n  type: http\n  scheme: bearer\n  surface: public REST API (https://api.car-cutter.com)\n  applied: root-level security on every operation\n  sources:\n  - openapi/meero-carcutter-openapi.json\n  detail: 'The scheme is named \"api_key\" but declared as HTTP bearer. Tokens are issued per\n    CarCutter account; there are no scopes, no token endpoint and no documented rotation or\n    expiry policy. The 401 message the contract publishes is \"submitted ''Bearer'' token is\n    unauthorized\".'\n  observed:\n    request: GET https://api.car-cutter.com/vehicle/status?vehicle_id=test\
  \ (no Authorization header)\n    http_status: 401\n    body_content_type: text/html\n    note: 'The live 401 body is an HTML \"401 Unauthorized\" page, not the JSON UnauthorizedResponse\n      the contract documents — a real gap between contract and runtime.'\n- name: none (public demo)\n  type: none\n  surface: POST https://api.car-cutter.com/vehicle/composition/segment\n  detail: 'A keyless demo composition path documented in github.com/carcutter/carcutter-api-samples.\n    Probed unauthenticated on 2026-08-25 and returned 400 \"invalid file\" rather than 401,\n    confirming it requires no credential. See sandbox/meero-sandbox.yml.'\n- name: carcutter_mcp_oauth\n  type: oauth2\n  surface: https://www.carcutter.com/wp-json/mcp/mcp-oauth-server\n  flows:\n    authorizationCode:\n      authorizationUrl: https://www.carcutter.com/oauth/authorize\n      tokenUrl: https://www.carcutter.com/oauth/token\n      refreshUrl: https://www.carcutter.com/oauth/token\n      scopes:\n        mcp: Access\
  \ to the CarCutter MCP server resource.\n  pkce: S256\n  client_registration: client_id_metadata_document (no client secret)\n  discovery:\n  - https://www.carcutter.com/.well-known/oauth-authorization-server\n  - https://www.carcutter.com/.well-known/oauth-protected-resource\n  detail: RFC 8414 + RFC 9728 compliant; the MCP 401 returns a WWW-Authenticate header pointing at the protected-resource metadata.\n- name: carcutter_hub_oidc\n  type: openIdConnect\n  openIdConnectUrl: https://auth.eu.car-cutter.com/.well-known/openid-configuration\n  surface: CarCutter Hub (https://hub.car-cutter.com/) and the gated audience https://api2.car-cutter.com\n  provider: Auth0\n  pkce: [S256, plain]\n  scopes_requested_by_hub: [openid, offline_access]\n  detail: 'Discovered from the Hub login redirect. api2.car-cutter.com is an AWS API Gateway that\n    answers every path with 403 {\"message\":\"Missing Authentication Token\"} — there is no public\n    contract for it, so it is recorded but not profiled.'\n\
  gaps:\n- No token rotation, expiry or revocation policy is published for the REST bearer token.\n- The REST API has no scopes; a token is all-or-nothing for the account.\n- No mutual TLS, no request signing, no IP allowlisting is documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/authentication/meero-authentication.yml
summary_line: http/oauth2/openIdConnect · 4 schemes
tags:
- Automotive
- Images
- Artificial Intelligence
- Computer Vision
- Photography
- Media Processing
- E-Commerce
- Vehicle Merchandising
- Company
---
