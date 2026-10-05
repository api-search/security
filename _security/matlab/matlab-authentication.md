---
anonymous_access: true
api_key_in: []
api_specs:
- filename: openapi-productionserver
  format: yaml
  label: MATLAB Production Server RESTful API
  slug: matlab-production-server-restful-api
  spec_type: OpenAPI
  url: https://github.com/mathworks-ref-arch/openapi-productionserver
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Matlab Authentication
name_suffix: Authentication
oauth_flows: []
overview: MATLAB declares 7 security scheme(s) across its OpenAPI definitions.
provider_name: MATLAB
provider_slug: matlab
scheme_count: 7
schemes:
- also_accepted_in: header (THINGSPEAKAPIKEY)
  api: ThingSpeak REST API
  docs: https://www.mathworks.com/help/thingspeak/get-a-channel-feed.html
  id: thingspeak_read_api_key
  in: query
  name: api_key
  note: Public channels can be read with no key at all — https://api.thingspeak.com/channels/9/feeds.json returned 200 with data anonymously on 2026-09-14.
  required: false
  scope_of_use: Reading data from a private channel.
  type: apiKey
- also_accepted_in: header (THINGSPEAKAPIKEY)
  api: ThingSpeak REST API
  docs: https://www.mathworks.com/help/thingspeak/write-data.html
  id: thingspeak_write_api_key
  in: query
  name: api_key
  required: true
  scope_of_use: Writing entries to a channel (/update, bulk JSON/CSV writes).
  type: apiKey
- api: ThingSpeak REST API
  docs: https://www.mathworks.com/help/thingspeak/channels-and-charts-api.html
  id: thingspeak_user_api_key
  in: query
  name: api_key
  required: true
  scope_of_use: Account-level operations — listing a user's channels, creating, updating and deleting channels.
  type: apiKey
- api: ThingSpeak MQTT API
  credentials:
  - client ID
  - username
  - password
  docs: https://www.mathworks.com/help/thingspeak/mqtt-basics.html
  id: thingspeak_mqtt_device
  limits:
    authorized_channels_per_device: 10
    devices_per_user: 100
  provisioning: Devices are created in the ThingSpeak web interface; regenerating credentials disables the old password.
  scope_of_use: Publish and subscribe on ThingSpeak channels.
  transport: MQTT / MQTT over WebSocket
  type: credentials
- api: MATLAB Production Server RESTful API
  docs: https://www.mathworks.com/help/mps/restfuljson/restful-api.html
  id: mps_session_cookie
  in: header
  name: Cookie
  scope_of_use: Required for asynchronous requests so the client sticks to the server that holds the request state; the server sets it with Set-Cookie. Omitted for synchronous requests.
  type: cookie
- api: MATLAB Production Server RESTful API
  docs: https://www.mathworks.com/help/mps/server/security.html
  id: mps_transport_security
  scope_of_use: MATLAB Production Server is customer-hosted. Transport security, client certificate verification and access control are configured on the operator's own instance rather than by MathWorks, so there is no MathWorks-issued credential for this API.
  type: mutualTLS
- api: MATLAB MCP Server
  docs: https://github.com/matlab/matlab-mcp-server#security-considerations
  id: matlab_mcp_server_local
  scope_of_use: 'The official MCP server runs as a local stdio process. There is no token: the trust boundary is the operator''s machine and the MATLAB licence on it. MathWorks'' own README asks for a human in the loop on every tool call because evaluate_matlab_code and run_matlab_file execute arbitrary code.'
  type: none
slug: matlab-authentication
source_filename: matlab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: MATLAB\nproviderId: matlab\ngenerated: '2026-09-14'\nmethod: searched\nsource: >-\n  https://www.mathworks.com/help/thingspeak/rest-api.html,\n  https://www.mathworks.com/help/thingspeak/get-a-channel-feed.html,\n  https://www.mathworks.com/help/thingspeak/mqtt-basics.html,\n  https://www.mathworks.com/help/mps/restfuljson/restful-api.html,\n  https://github.com/matlab/matlab-mcp-server\nnote: >-\n  Not derived from an OpenAPI: MathWorks publishes no OpenAPI/Swagger document for any of these\n  surfaces (see x-coverage in apis.yml). Every scheme below was read from the provider's own docs.\n  There is no OAuth 2.0 or OpenID Connect anywhere on the public API surface — /.well-known/openid-configuration\n  and /.well-known/oauth-authorization-server are not served on any MathWorks host (see well-known/matlab-well-known.yml),\n  so scopes/ is deliberately absent rather than empty.\noauth2: false\n\
  openid_connect: false\nschemes:\n  - id: thingspeak_read_api_key\n    api: ThingSpeak REST API\n    type: apiKey\n    in: query\n    name: api_key\n    also_accepted_in: header (THINGSPEAKAPIKEY)\n    scope_of_use: Reading data from a private channel.\n    required: false\n    note: Public channels can be read with no key at all — https://api.thingspeak.com/channels/9/feeds.json returned 200 with data anonymously on 2026-09-14.\n    docs: https://www.mathworks.com/help/thingspeak/get-a-channel-feed.html\n  - id: thingspeak_write_api_key\n    api: ThingSpeak REST API\n    type: apiKey\n    in: query\n    name: api_key\n    also_accepted_in: header (THINGSPEAKAPIKEY)\n    scope_of_use: Writing entries to a channel (/update, bulk JSON/CSV writes).\n    required: true\n    docs: https://www.mathworks.com/help/thingspeak/write-data.html\n  - id: thingspeak_user_api_key\n    api: ThingSpeak REST API\n    type: apiKey\n    in: query\n    name: api_key\n    scope_of_use: Account-level operations\
  \ — listing a user's channels, creating, updating and deleting channels.\n    required: true\n    docs: https://www.mathworks.com/help/thingspeak/channels-and-charts-api.html\n  - id: thingspeak_mqtt_device\n    api: ThingSpeak MQTT API\n    type: credentials\n    transport: MQTT / MQTT over WebSocket\n    credentials:\n      - client ID\n      - username\n      - password\n    scope_of_use: Publish and subscribe on ThingSpeak channels.\n    provisioning: Devices are created in the ThingSpeak web interface; regenerating credentials disables the old password.\n    limits:\n      authorized_channels_per_device: 10\n      devices_per_user: 100\n    docs: https://www.mathworks.com/help/thingspeak/mqtt-basics.html\n  - id: mps_session_cookie\n    api: MATLAB Production Server RESTful API\n    type: cookie\n    in: header\n    name: Cookie\n    scope_of_use: >-\n      Required for asynchronous requests so the client sticks to the server that holds the request\n      state; the server sets it\
  \ with Set-Cookie. Omitted for synchronous requests.\n    docs: https://www.mathworks.com/help/mps/restfuljson/restful-api.html\n  - id: mps_transport_security\n    api: MATLAB Production Server RESTful API\n    type: mutualTLS\n    scope_of_use: >-\n      MATLAB Production Server is customer-hosted. Transport security, client certificate verification\n      and access control are configured on the operator's own instance rather than by MathWorks, so\n      there is no MathWorks-issued credential for this API.\n    docs: https://www.mathworks.com/help/mps/server/security.html\n  - id: matlab_mcp_server_local\n    api: MATLAB MCP Server\n    type: none\n    scope_of_use: >-\n      The official MCP server runs as a local stdio process. There is no token: the trust boundary is\n      the operator's machine and the MATLAB licence on it. MathWorks' own README asks for a human in\n      the loop on every tool call because evaluate_matlab_code and run_matlab_file execute arbitrary code.\n   \
  \ docs: https://github.com/matlab/matlab-mcp-server#security-considerations\ntransport:\n  https_required: true\n  evidence: >-\n    ThingSpeak and mathworks.com both negotiate TLSv1.3; see security/matlab-domain-security.yml.\n    ThingSpeak additionally rejects REST requests whose Host header is not api.thingspeak.com.\nkey_management:\n  rotation: Channel Read/Write API keys and MQTT device credentials are regenerable from the ThingSpeak web interface.\n  documented_prefixes: none\n  expiry: none documented\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matlab/refs/heads/main/authentication/matlab-authentication.yml
summary_line: 7 schemes
tags:
- Data Analysis
- Engineering
- Machine Learning
- Numerical Analysis
- Scientific Computing
---
