---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: red5-webrtc-streaming-asyncapi.yml
  format: yaml
  label: Red5 Pro WebRTC SDK
  slug: webrtc-sdk
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/asyncapi/red5-webrtc-streaming-asyncapi.yml
- filename: red5-admin-api-openapi.yml
  format: yaml
  label: Red5 Admin API
  slug: red5-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-admin-api-openapi.yml
- filename: red5-file-restreamer-api-openapi.yml
  format: yaml
  label: Red5 File Restreamer API
  slug: red5-file-restreamer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-file-restreamer-api-openapi.yml
- filename: red5-images-api-openapi.yml
  format: yaml
  label: Red5 Images API
  slug: red5-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-images-api-openapi.yml
- filename: red5-inputs-api-openapi.yml
  format: yaml
  label: Red5 Inputs API
  slug: red5-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-inputs-api-openapi.yml
- filename: red5-mixers-api-openapi.yml
  format: yaml
  label: Red5 Mixers API
  slug: red5-mixers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-mixers-api-openapi.yml
- filename: red5-provision-api-openapi.yml
  format: yaml
  label: Red5 Provision API
  slug: red5-provision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-provision-api-openapi.yml
- filename: red5-proxy-api-openapi.yml
  format: yaml
  label: Red5 Proxy API
  slug: red5-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-proxy-api-openapi.yml
- filename: red5-rtmp-restreamer-api-openapi.yml
  format: yaml
  label: Red5 RTMP Restreamer API
  slug: red5-rtmp-restreamer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-rtmp-restreamer-api-openapi.yml
- filename: red5-servlet-configuration-api-openapi.yml
  format: yaml
  label: Red5 Servlet Configuration API
  slug: red5-servlet-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-servlet-configuration-api-openapi.yml
- filename: red5-streams-api-openapi.yml
  format: yaml
  label: Red5 Streams API
  slug: red5-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/openapi/red5-streams-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Red5 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Red5 secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Red5
provider_slug: red5
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT bearer token for authenticating Stream Manager API requests
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/red5-admin-api-openapi.yml
  - openapi/red5-provision-api-openapi.yml
  - openapi/red5-proxy-api-openapi.yml
  - openapi/red5-streams-api-openapi.yml
  type: http
- description: API access token for authenticating Restreamer API requests
  in: query
  name: accessToken
  parameter: accessToken
  sources:
  - openapi/red5-file-restreamer-api-openapi.yml
  - openapi/red5-images-api-openapi.yml
  - openapi/red5-inputs-api-openapi.yml
  - openapi/red5-mixers-api-openapi.yml
  - openapi/red5-rtmp-restreamer-api-openapi.yml
  - openapi/red5-servlet-configuration-api-openapi.yml
  type: apiKey
slug: red5-authentication
source_filename: red5-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: openapi/red5-admin-api-openapi.yml, openapi/red5-file-restreamer-api-openapi.yml, openapi/red5-images-api-openapi.yml,\n  openapi/red5-inputs-api-openapi.yml, openapi/red5-mixers-api-openapi.yml, openapi/red5-provision-api-openapi.yml,\n  openapi/red5-proxy-api-openapi.yml, openapi/red5-rtmp-restreamer-api-openapi.yml, openapi/red5-servlet-configuration-api-openapi.yml,\n  openapi/red5-streams-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT bearer token for authenticating Stream Manager API requests\n  sources:\n  - openapi/red5-admin-api-openapi.yml\n  - openapi/red5-provision-api-openapi.yml\n  - openapi/red5-proxy-api-openapi.yml\n  - openapi/red5-streams-api-openapi.yml\n- name: accessToken\n  type: apiKey\n  in: query\n  parameter: accessToken\n  description: API access token for authenticating\
  \ Restreamer API requests\n  sources:\n  - openapi/red5-file-restreamer-api-openapi.yml\n  - openapi/red5-images-api-openapi.yml\n  - openapi/red5-inputs-api-openapi.yml\n  - openapi/red5-mixers-api-openapi.yml\n  - openapi/red5-rtmp-restreamer-api-openapi.yml\n  - openapi/red5-servlet-configuration-api-openapi.yml\ndocs: https://www.red5.net/docs/red5-pro/users-guide/authentication/\ndocs_additional:\n- https://www.red5.net/docs/red5-cloud/users-guide/authentication/\n- https://www.red5.net/docs/red5-cloud/users-guide/authentication/red5-cloud-digest-token-authentication/\n- https://www.red5.net/docs/red5-cloud/users-guide/authentication/red5-cloud-round-trip-authentication/\n- https://www.red5.net/docs/red5-pro/development/api/authentication/\n- https://www.red5.net/docs/red5-cloud/development/sdks/backend-sdk/\nnote: Upgraded from derived to searched 2026-09-04. The two OpenAPI-declared schemes below cover only\n  the control plane. Red5's real authentication story has a second half\
  \ the specs do not carry — the MEDIA\n  PLANE, where publish/subscribe credentials travel in the client SDK's connectionParams (username / password\n  / token) rather than in an HTTP header, and where the mechanism differs between the self-hosted and\n  managed products.\nmedia_plane:\n  red5_pro_self_hosted:\n  - name: Round Trip Authentication\n    class: RoundTripAuthValidator\n    description: Red5 asks a customer-operated remote validation service to authorize each publish or\n      subscribe request; the service returns a JSON result. Clients missing username/password/token entirely\n      are rejected at connect time, before the round trip fires. Publishers and subscribers are authenticated\n      distinctly by role.\n    docs: https://www.red5.net/docs/red5-pro/users-guide/authentication/\n  - name: JWT Authentication\n    class: JwtAuthenticator\n    description: RFC 7519 tokens validated LOCALLY with standard libraries and signatures — no remote\n      call per request. Validates\
  \ expiration, issuer, roles, transport restrictions and room restrictions.\n    standard: RFC 7519\n  - name: Simple Authentication\n    plugin: red5pro-simple-auth-plugin\n    description: Connection-level (not action-level) username/password checking for RTMP, RTSP and WebRTC\n      clients. Configurable per webapp via red5-web.xml or globally via simple-auth-plugin.credentials\n      in RED5_HOME/conf, and tunable independently per connection type.\n  red5_cloud_managed:\n  - name: Round Trip Authentication (Cloud)\n    description: Same concept as standalone, but wired up per node group in the Red5 Cloud UI by pointing\n      at a validation server URL instead of editing red5-web.xml. Requires a node image built with the\n      Simple Auth plugin. The validator implements validateCredentials / invalidateCredentials HTTP POST\n      endpoints.\n  - name: Digest Token Authentication\n    cloud_only: true\n    description: 'Self-contained cryptographically signed token — no callback to\
  \ an external server. Seven\n      colon-separated fields: stream:user:role:key1=value1:app:expiration:digest, where stream is the\n      SHORT stream id (stream1, not live/stream1), role is streamer or viewer, expiration is a Unix timestamp,\n      and digest is sha256(payload + \":\" + secret) as 64-char lowercase hex over the first six fields.\n      Configured per node group in the Cloud UI (Digest Algorithm SHA-256 plus the shared secret).'\n    common_failure: A secret mismatch between the Cloud UI and the token generator rejects every connection.\n  transport_note: 'On WebRTC/WHIP/WHEP the credential is passed through the SDK''s connectionParams init\n    property — connectionParams: { username, password, token } — not a query string. The WHIP/WHEP endpoint\n    uses the FULL stream path (/live/stream1) while a Digest Token''s stream field uses only the short\n    id (stream1).'\ntoken_minting:\n  backend_sdks:\n  - red5-bcs-node (npm, published)\n  - net.red5:red5-bcs-java (documented,\
  \ not on Maven Central)\n  - github.com/red5pro/red5-bcs-go (documented, module not public)\n  description: 'Red5 Cloud Backend SDKs mint short-lived role-scoped tokens server-side from a master\n    key and master secret: getConferenceToken(userId, roomId, role, expirationMinutes) with role admin\n    / publisher / subscriber, and getChatToken(userId, channelId, read, write, ttlMinutes). Red5 documents\n    these as a separate mechanism from the standalone JwtAuthenticator path.'\n  guidance:\n  - Store master credentials in environment variables, never in client code.\n  - Never generate tokens on the client.\n  - Use HTTPS.\n  - Keep token lifetimes short.\n  - Validate users before issuing tokens.\noauth2:\n  supported: false\n  evidence: derive-oauth-scopes.py 2026-09-04 found 0 oauth2 schemes and 0 scopes across all ten specs;\n    /.well-known/openid-configuration 404s on every Red5-owned host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/authentication/red5-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Live Streaming
- Media
- Real-Time
- RTMP
- Streaming
- Video
- WebRTC
---
