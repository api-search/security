---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Quanergy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quanergy declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Quanergy
provider_slug: quanergy
scheme_count: 3
schemes:
- credential_policy:
    account_expiry: The server pushes `Security/Expiring` (with an `hours` parameter) and `Security/Expired` gRPC notifications for user accounts, so accounts have a finite lifetime.
    password_composition: upper and lower case letters plus digits
    password_min_length: 6
    username_composition: letters and digits
    username_min_length: 4
  description: 'RFC 7616-style HTTP Digest access authentication against the QORTEX HTTP command server. Two-phase GET: the first request draws a nonce, the second carries the digest hash. Credentials may be a username/password pair or a License ID/License password pair; the documentation recommends username auth and treats the License ID as an administrative backup path.'
  endpoint: https://<IP_Address>:8080/v1/login
  id: http-digest
  realm: realm@quanergy
  scheme: digest
  type: http
  x-note: The published Python example calls the login endpoint over plain `http://` on port 8080 while the prose gives the endpoint as `https://`. Both forms appear in Rev A.
- commands:
  - authenticated: false
    command: GetSecured
    description: Reports whether the QORTEX DTC system is currently secured and whether a username is configured. This is the only command that does not require authentication.
    response_headers:
    - Q-Secured
    - Q-UserPresent
  - authenticated: true
    command: GetToken
    description: Returns a 64-character hex token which is unhexed into the AES-256 key used to decrypt the TCP publisher streams. Failure returns HTTP 401.
    response_headers:
    - Q-Token
  - authenticated: true
    command: SetSecured:true|false
    description: Secures or unsecures the whole client-to-server data flow. Reply is `ok` or `failed`.
    response_headers:
    - Q-SetSecured
  - authenticated: true
    command: SetCredentials:username:encryptedPassword
    description: Sets user credentials using the documented HTTP password encryption formula; on success returns true plus a security token.
    response_headers:
    - Q-CredentialsSet
    - Q-Token
  description: A custom application-level command header layered on top of HTTP Digest. One command per request, parameters delimited by colons. Server replies come back on `Q-*` headers.
  id: q-auth-header
  in: header
  name: Q-Auth
  type: apiKey
- description: Every gRPC call carries a `client_id` metadata pair holding the string form of a 128-bit UUID. This is how the QORTEX DTC server distinguishes concurrent clients. It is an identity/correlation value, not a credential — authentication is carried by the Q-Auth / Digest exchange when Security mode is on.
  endpoint: <IP_Address>:17177
  id: grpc-client-id-metadata
  metadata_key: client_id
  transport: grpc
  type: metadata
  x-example-shape: metadata = (("client_id", "<uuid4>"),)
slug: quanergy-authentication
source_filename: quanergy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://downloads.quanergy.com/qortex/Qortex-API-Reference-RevA-120824.pdf\ndocs: https://downloads.quanergy.com/qortex/Qortex-API-Reference-RevA-120824.pdf\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://downloads.quanergy.com/qortex/Qortex-API-Reference-RevA-120824.pdf\n  http_status: 200\n  content_type: application/pdf\n  document: QORTEX DTC for Q-Track API Reference, QPN 96-00134 Rev A (2024-09-15)\n\napi: QORTEX DTC API\ndeployment: on-premises\ndefault_posture: >-\n  Security mode is OFF by default on the QORTEX DTC server. When Security mode is disabled the\n  gRPC endpoint (port 17177) and the TCP publisher ports are unauthenticated and unencrypted on\n  the local network. Security mode is enabled by an operator from the QORTEX DTC client in\n  Configuration mode and requires an activated Quanergy license.\n\nschemes:\n  - id: http-digest\n    type: http\n    scheme: digest\n    realm: realm@quanergy\n    endpoint:\
  \ 'https://<IP_Address>:8080/v1/login'\n    description: >-\n      RFC 7616-style HTTP Digest access authentication against the QORTEX HTTP command server.\n      Two-phase GET: the first request draws a nonce, the second carries the digest hash.\n      Credentials may be a username/password pair or a License ID/License password pair; the\n      documentation recommends username auth and treats the License ID as an administrative\n      backup path.\n    credential_policy:\n      username_min_length: 4\n      username_composition: letters and digits\n      password_min_length: 6\n      password_composition: upper and lower case letters plus digits\n      account_expiry: >-\n        The server pushes `Security/Expiring` (with an `hours` parameter) and `Security/Expired`\n        gRPC notifications for user accounts, so accounts have a finite lifetime.\n    x-note: >-\n      The published Python example calls the login endpoint over plain `http://` on port 8080\n      while the prose gives\
  \ the endpoint as `https://`. Both forms appear in Rev A.\n\n  - id: q-auth-header\n    type: apiKey\n    in: header\n    name: Q-Auth\n    description: >-\n      A custom application-level command header layered on top of HTTP Digest. One command per\n      request, parameters delimited by colons. Server replies come back on `Q-*` headers.\n    commands:\n      - command: GetSecured\n        authenticated: false\n        response_headers: [Q-Secured, Q-UserPresent]\n        description: >-\n          Reports whether the QORTEX DTC system is currently secured and whether a username is\n          configured. This is the only command that does not require authentication.\n      - command: GetToken\n        authenticated: true\n        response_headers: [Q-Token]\n        description: >-\n          Returns a 64-character hex token which is unhexed into the AES-256 key used to decrypt\n          the TCP publisher streams. Failure returns HTTP 401.\n      - command: 'SetSecured:true|false'\n\
  \        authenticated: true\n        response_headers: [Q-SetSecured]\n        description: Secures or unsecures the whole client-to-server data flow. Reply is `ok` or `failed`.\n      - command: 'SetCredentials:username:encryptedPassword'\n        authenticated: true\n        response_headers: [Q-CredentialsSet, Q-Token]\n        description: >-\n          Sets user credentials using the documented HTTP password encryption formula; on success\n          returns true plus a security token.\n\n  - id: grpc-client-id-metadata\n    type: metadata\n    transport: grpc\n    endpoint: '<IP_Address>:17177'\n    metadata_key: client_id\n    description: >-\n      Every gRPC call carries a `client_id` metadata pair holding the string form of a 128-bit\n      UUID. This is how the QORTEX DTC server distinguishes concurrent clients. It is an\n      identity/correlation value, not a credential — authentication is carried by the Q-Auth /\n      Digest exchange when Security mode is on.\n    x-example-shape:\
  \ 'metadata = ((\"client_id\", \"<uuid4>\"),)'\n\nauthorization:\n  model: mode-based\n  description: >-\n    Authorization is not scope- or role-based. Each gRPC method belongs to either Monitor mode\n    or Config mode. A client must hold an open `SwitchToConfigMode` bidirectional stream before\n    calling any Config-mode method, otherwise the server returns a permission-denied error.\n  modes:\n    - name: monitor\n      requires_switch_to_config_mode: false\n      methods:\n        - GetZones\n        - GetEventZoneViolationActions\n        - GetEventZoneViolationRecordingEnabled\n        - GetEventZoneViolationHandlerEnabled\n        - GetServerState\n        - GetSensorState\n        - GetFile\n        - PubSub\n    - name: config\n      requires_switch_to_config_mode: true\n      description: >-\n        Every remaining method — zone, counter-line, rule, PTZ camera, settings, recording and\n        playback configuration — requires the client to hold the Config-mode stream.\n \
  \ entitlements:\n    - name: SubVehicle license add-on\n      effect: >-\n        Without it the tracker emits only PERSON, VEHICLE and UNKNOWN classifications.\n        TWOWHEELER_VEHICLE, PASSENGER_VEHICLE and COMMERCIAL_VEHICLE are only populated when the\n        sub-classification license is present.\n\ntransport_security:\n  - control: AES-256 payload encryption\n    applies_to: [object/trackable list, zone list, sensor health/state list]\n    description: >-\n      When Security mode is on, the TCP publisher payloads are AES-256 encrypted. The key is the\n      unhexed `Q-Token`. Quanergy ships Python and C++ TCP listener samples that perform the\n      decryption; the corresponding publisher must be configured with\n      `<TCPPublisher><AddDataSize>true</AddDataSize></TCPPublisher>`.\n  - control: no CA required\n    description: >-\n      The documentation states explicitly that internet access and a Certificate Authority are\n      not required — the scheme is self-contained\
  \ on the customer network.\n\nnot_present:\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  - api-key-issuance-portal\n  - self-service-credentials\n\ngaps:\n  - >-\n    Security mode being off by default means a stock QORTEX DTC deployment publishes person and\n    vehicle track data on unauthenticated TCP ports. The default is a deployment-hardening\n    decision for the operator, but it is not called out as a hardening step in the API Reference.\n  - >-\n    No machine-readable description of the auth surface is published — no OpenAPI for the\n    port-8080 HTTP command server, and no `.proto` for the gRPC service.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quanergy/refs/heads/main/authentication/quanergy-authentication.yml
summary_line: 3 schemes
tags:
- Company
- LiDAR
- Sensors
- Physical Security
- Perimeter Security
- Perception
- Crowd Management
- Industrial Automation
- Internet of Things
- gRPC
- Streaming
- Hardware
---
