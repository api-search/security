---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Innovusion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seyond declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Seyond
provider_slug: innovusion
scheme_count: 3
schemes:
- bearer_methods:
  - header
  client_registration: client_id_metadata_document
  discovery:
  - https://seyond.com/.well-known/oauth-authorization-server
  - https://seyond.com/.well-known/oauth-protected-resource
  evidence:
    challenge_header: 'WWW-Authenticate: Bearer realm="https://seyond.com", resource_metadata="https://seyond.com/.well-known/oauth-protected-resource"'
    challenge_status: 401
  flows:
    authorizationCode:
      authorizationUrl: https://seyond.com/oauth/authorize
      refreshUrl: null
      revocationUrl: https://seyond.com/oauth/revoke
      scopes:
        mcp: The single scope advertised by the authorization server for MCP access.
      tokenUrl: https://seyond.com/oauth/token
  id: mcp-oauth2
  pkce:
    required_methods:
    - S256
  surface: https://seyond.com/wp-json/mcp/mcp-oauth-server
  token_endpoint_auth_methods:
  - none
  type: oauth2
- id: wordpress-session
  note: The second registered MCP server rejects anonymous calls with the WordPress REST rest_forbidden envelope rather than an OAuth challenge, so it is gated on a logged-in WordPress session/nonce (X-WP-Nonce is in the Access-Control-Allow-Headers list) rather than on a bearer token.
  surface: https://seyond.com/wp-json/mcp/mcp-adapter-default-server
  type: cookie
- evidence:
  - https://github.com/Seyond-Inc/inno-lidar-sdk/blob/main/docs/HOW_TO_USE_CLIENT_SDK.md
  - https://github.com/Seyond-Inc/inno-lidar-sdk/blob/main/src/sdk_common/lidar_communication.h
  id: device-local-none
  note: The client SDK connects to a sensor on the local network by IP address and port (inno_lidar_open_live(name, lidar_ip, port, protocol, udp_port)). The SDK exposes no credential parameter and the published documentation describes none, so the sensor command and point-cloud channels are unauthenticated network services and their security depends on network segmentation. Recorded as observed from the published SDK source and docs, not as a recommendation.
  surface: LiDAR sensor command channel (inno-lidar-sdk)
  type: none
slug: innovusion-authentication
source_filename: innovusion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://seyond.com/.well-known/oauth-authorization-server\nnote: >-\n  There is no OpenAPI to derive securitySchemes from — derive-authentication.py found no spec for this\n  provider. This profile is built entirely from live probes of the surfaces Seyond actually serves.\n  Seyond publishes no API key programme, no developer signup and no documented authentication page.\nschemes:\n- id: mcp-oauth2\n  type: oauth2\n  surface: https://seyond.com/wp-json/mcp/mcp-oauth-server\n  flows:\n    authorizationCode:\n      authorizationUrl: https://seyond.com/oauth/authorize\n      tokenUrl: https://seyond.com/oauth/token\n      refreshUrl: null\n      revocationUrl: https://seyond.com/oauth/revoke\n      scopes:\n        mcp: The single scope advertised by the authorization server for MCP access.\n  pkce:\n    required_methods: [S256]\n  token_endpoint_auth_methods: [none]\n  client_registration: client_id_metadata_document\n  bearer_methods:\
  \ [header]\n  discovery:\n  - https://seyond.com/.well-known/oauth-authorization-server\n  - https://seyond.com/.well-known/oauth-protected-resource\n  evidence:\n    challenge_header: >-\n      WWW-Authenticate: Bearer realm=\"https://seyond.com\",\n      resource_metadata=\"https://seyond.com/.well-known/oauth-protected-resource\"\n    challenge_status: 401\n- id: wordpress-session\n  type: cookie\n  surface: https://seyond.com/wp-json/mcp/mcp-adapter-default-server\n  note: >-\n    The second registered MCP server rejects anonymous calls with the WordPress REST rest_forbidden\n    envelope rather than an OAuth challenge, so it is gated on a logged-in WordPress session/nonce\n    (X-WP-Nonce is in the Access-Control-Allow-Headers list) rather than on a bearer token.\n- id: device-local-none\n  type: none\n  surface: LiDAR sensor command channel (inno-lidar-sdk)\n  note: >-\n    The client SDK connects to a sensor on the local network by IP address and port\n    (inno_lidar_open_live(name,\
  \ lidar_ip, port, protocol, udp_port)). The SDK exposes no credential\n    parameter and the published documentation describes none, so the sensor command and point-cloud\n    channels are unauthenticated network services and their security depends on network segmentation.\n    Recorded as observed from the published SDK source and docs, not as a recommendation.\n  evidence:\n  - https://github.com/Seyond-Inc/inno-lidar-sdk/blob/main/docs/HOW_TO_USE_CLIENT_SDK.md\n  - https://github.com/Seyond-Inc/inno-lidar-sdk/blob/main/src/sdk_common/lidar_communication.h\nunauthenticated_surfaces:\n- url: https://api.seyond.com/health\n  status: 200\n  body: ok\n  note: The only path on the SIMPL API host that answers; every other probed path returns nginx 404.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innovusion/refs/heads/main/authentication/innovusion-authentication.yml
summary_line: 3 schemes
tags:
- Company
- LiDAR
- Sensors
- Autonomous Driving
- Intelligent Transportation
- Robotics
- Perception
- Smart Cities
- Automotive
- Hardware
---
