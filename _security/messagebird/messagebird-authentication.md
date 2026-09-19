---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: messagebird-bird-api-openapi.yml
  format: yaml
  label: Bird API
  slug: bird-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-bird-api-openapi.yml
- filename: messagebird-available-numbers-api-openapi.yml
  format: yaml
  label: messagebird Available Numbers API
  slug: messagebird-available-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-available-numbers-api-openapi.yml
- filename: messagebird-balance-api-openapi.yml
  format: yaml
  label: messagebird Balance API
  slug: messagebird-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-balance-api-openapi.yml
- filename: messagebird-call-flows-api-openapi.yml
  format: yaml
  label: messagebird Call Flows API
  slug: messagebird-call-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-call-flows-api-openapi.yml
- filename: messagebird-calls-api-openapi.yml
  format: yaml
  label: messagebird Calls API
  slug: messagebird-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-calls-api-openapi.yml
- filename: messagebird-contacts-api-openapi.yml
  format: yaml
  label: messagebird Contacts API
  slug: messagebird-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-contacts-api-openapi.yml
- filename: messagebird-conversations-api-openapi.yml
  format: yaml
  label: messagebird Conversations API
  slug: messagebird-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-conversations-api-openapi.yml
- filename: messagebird-groups-api-openapi.yml
  format: yaml
  label: messagebird Groups API
  slug: messagebird-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-groups-api-openapi.yml
- filename: messagebird-hlr-api-openapi.yml
  format: yaml
  label: messagebird HLR API
  slug: messagebird-hlr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-hlr-api-openapi.yml
- filename: messagebird-legs-api-openapi.yml
  format: yaml
  label: messagebird Legs API
  slug: messagebird-legs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-legs-api-openapi.yml
- filename: messagebird-lookup-api-openapi.yml
  format: yaml
  label: messagebird Lookup API
  slug: messagebird-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-lookup-api-openapi.yml
- filename: messagebird-messages-api-openapi.yml
  format: yaml
  label: messagebird Messages API
  slug: messagebird-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-messages-api-openapi.yml
- filename: messagebird-purchased-numbers-api-openapi.yml
  format: yaml
  label: messagebird Purchased Numbers API
  slug: messagebird-purchased-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-purchased-numbers-api-openapi.yml
- filename: messagebird-recordings-api-openapi.yml
  format: yaml
  label: messagebird Recordings API
  slug: messagebird-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-recordings-api-openapi.yml
- filename: messagebird-templates-api-openapi.yml
  format: yaml
  label: messagebird Templates API
  slug: messagebird-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-templates-api-openapi.yml
- filename: messagebird-transcriptions-api-openapi.yml
  format: yaml
  label: messagebird Transcriptions API
  slug: messagebird-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-transcriptions-api-openapi.yml
- filename: messagebird-verify-api-openapi.yml
  format: yaml
  label: messagebird Verify API
  slug: messagebird-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-verify-api-openapi.yml
- filename: messagebird-voice-messages-api-openapi.yml
  format: yaml
  label: messagebird Voice Messages API
  slug: messagebird-voice-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-voice-messages-api-openapi.yml
- filename: messagebird-webhooks-api-openapi.yml
  format: yaml
  label: messagebird Webhooks API
  slug: messagebird-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Messagebird Authentication
name_suffix: Authentication
oauth_flows: []
overview: Messagebird secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Messagebird
provider_slug: messagebird
scheme_count: 5
schemes:
- description: Access key authentication in the form of 'AccessKey {accessKey}'.
  in: header
  name: accessKey
  parameter: Authorization
  sources:
  - openapi/messagebird-available-numbers-api-openapi.yml
  - openapi/messagebird-balance-api-openapi.yml
  - openapi/messagebird-call-flows-api-openapi.yml
  - openapi/messagebird-calls-api-openapi.yml
  - openapi/messagebird-contacts-api-openapi.yml
  - openapi/messagebird-conversations-api-openapi.yml
  - openapi/messagebird-groups-api-openapi.yml
  - openapi/messagebird-hlr-api-openapi.yml
  - openapi/messagebird-legs-api-openapi.yml
  - openapi/messagebird-lookup-api-openapi.yml
  - openapi/messagebird-messages-api-openapi.yml
  - openapi/messagebird-purchased-numbers-api-openapi.yml
  - openapi/messagebird-recordings-api-openapi.yml
  - openapi/messagebird-templates-api-openapi.yml
  - openapi/messagebird-transcriptions-api-openapi.yml
  - openapi/messagebird-verify-api-openapi.yml
  - openapi/messagebird-voice-messages-api-openapi.yml
  - openapi/messagebird-webhooks-api-openapi.yml
  type: apiKey
- description: 'Pass the API key as a bearer token in the `Authorization` header. Keys use

    the format `bk_{region}_*`. The prefix identifies the region and selects the

    API endpoint. Official Bird SDKs and the CLI derive the region from the key.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/messagebird-bird-api-openapi.yml
  type: http
- description: 'Session cookie set after signing in to the Bird dashboard. The cookie

    value is an opaque session token; no session data is stored in the cookie

    itself.'
  in: cookie
  name: CookieAuth
  parameter: bird_session
  sources:
  - openapi/messagebird-bird-api-openapi.yml
  type: apiKey
- description: 'The Realtime app key. Together with `X-Realtime-Secret`, it authenticates a

    request to the Realtime API in addition to the workspace credential. Both

    values come from the app''s credentials and must belong to the calling

    workspace. Official Bird SDKs accept the pair as client configuration.'
  in: header
  name: RealtimeKey
  parameter: X-Realtime-Key
  sources:
  - openapi/messagebird-bird-api-openapi.yml
  type: apiKey
- description: 'The Realtime app secret paired with `X-Realtime-Key`. The API returns the

    secret only when the key is created and does not store it. Create a new key

    and revoke the current key if you lose the secret. Official Bird SDKs accept

    the pair as client configuration.'
  in: header
  name: RealtimeSecret
  parameter: X-Realtime-Secret
  sources:
  - openapi/messagebird-bird-api-openapi.yml
  type: apiKey
slug: messagebird-authentication
source_filename: messagebird-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: openapi/messagebird-available-numbers-api-openapi.yml, openapi/messagebird-balance-api-openapi.yml, openapi/messagebird-bird-api-openapi.yml,\n  openapi/messagebird-call-flows-api-openapi.yml, openapi/messagebird-calls-api-openapi.yml, openapi/messagebird-contacts-api-openapi.yml,\n  openapi/messagebird-conversations-api-openapi.yml, openapi/messagebird-groups-api-openapi.yml, openapi/messagebird-hlr-api-openapi.yml,\n  openapi/messagebird-legs-api-openapi.yml, openapi/messagebird-lookup-api-openapi.yml, openapi/messagebird-messages-api-openapi.yml\n  ...\nsummary:\n  types:\n    - apiKey\n    - http\n  api_key_in:\n    - cookie\n    - header\nschemes:\n  - name: accessKey\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: Access key authentication in the form of 'AccessKey {accessKey}'.\n    sources:\n      - openapi/messagebird-available-numbers-api-openapi.yml\n      - openapi/messagebird-balance-api-openapi.yml\n\
  \      - openapi/messagebird-call-flows-api-openapi.yml\n      - openapi/messagebird-calls-api-openapi.yml\n      - openapi/messagebird-contacts-api-openapi.yml\n      - openapi/messagebird-conversations-api-openapi.yml\n      - openapi/messagebird-groups-api-openapi.yml\n      - openapi/messagebird-hlr-api-openapi.yml\n      - openapi/messagebird-legs-api-openapi.yml\n      - openapi/messagebird-lookup-api-openapi.yml\n      - openapi/messagebird-messages-api-openapi.yml\n      - openapi/messagebird-purchased-numbers-api-openapi.yml\n      - openapi/messagebird-recordings-api-openapi.yml\n      - openapi/messagebird-templates-api-openapi.yml\n      - openapi/messagebird-transcriptions-api-openapi.yml\n      - openapi/messagebird-verify-api-openapi.yml\n      - openapi/messagebird-voice-messages-api-openapi.yml\n      - openapi/messagebird-webhooks-api-openapi.yml\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    description: 'Pass the API key as a bearer token in the `Authorization`\
  \ header. Keys use\n\n      the format `bk_{region}_*`. The prefix identifies the region and selects the\n\n      API endpoint. Official Bird SDKs and the CLI derive the region from the key.'\n    sources:\n      - openapi/messagebird-bird-api-openapi.yml\n  - name: CookieAuth\n    type: apiKey\n    in: cookie\n    parameter: bird_session\n    description: 'Session cookie set after signing in to the Bird dashboard. The cookie\n\n      value is an opaque session token; no session data is stored in the cookie\n\n      itself.'\n    sources:\n      - openapi/messagebird-bird-api-openapi.yml\n  - name: RealtimeKey\n    type: apiKey\n    in: header\n    parameter: X-Realtime-Key\n    description: 'The Realtime app key. Together with `X-Realtime-Secret`, it authenticates a\n\n      request to the Realtime API in addition to the workspace credential. Both\n\n      values come from the app''s credentials and must belong to the calling\n\n      workspace. Official Bird SDKs accept the pair as client\
  \ configuration.'\n    sources:\n      - openapi/messagebird-bird-api-openapi.yml\n  - name: RealtimeSecret\n    type: apiKey\n    in: header\n    parameter: X-Realtime-Secret\n    description: 'The Realtime app secret paired with `X-Realtime-Key`. The API returns the\n\n      secret only when the key is created and does not store it. Create a new key\n\n      and revoke the current key if you lose the secret. Official Bird SDKs accept\n\n      the pair as client configuration.'\n    sources:\n      - openapi/messagebird-bird-api-openapi.yml\ndocs: https://bird.com/docs/guides/authentication\ndocs_agent: https://bird.com/auth.md\nsearched_notes:\n  - 'Bird platform API: bearer credential in the Authorization header. Two token families — API keys prefixed bk_{region}_\n    and OAuth access tokens prefixed bt_{region}_; the prefix names the region and therefore the host to call (us1.platform.bird.com\n    / eu1.platform.bird.com).'\n  - 'Bird is an OAuth 2.0 authorization server issuing\
  \ at https://platform.bird.com. Grants: authorization_code\n    with PKCE S256, device_code, refresh_token (rotating). No client_credentials and no assertion grant — an agent\n    always acts for a consenting user.'\n  - RFC 7591 dynamic client registration is open at https://platform.bird.com/v1/oauth/register; a registered client\n    is public and its client_name is self-asserted.\n  - 'A 401 names its own discovery document: WWW-Authenticate: Bearer resource_metadata=\"https://platform.bird.com/.well-known/oauth-protected-resource\".'\n  - 44 scopes, resource:level pairs, enumerated in scopes/messagebird-scopes.yml. Consent caps an over-broad request\n    down to what the user holds rather than refusing it.\n  - Realtime uses a separate app key/secret pair (X-Realtime-Key / X-Realtime-Secret) alongside the workspace credential.\n  - 'The legacy MessageBird REST API (rest.messagebird.com) is unrelated: Authorization: AccessKey {accessKey},\n    no OAuth, no scopes.'\nsee_also:\n  -\
  \ scopes/messagebird-scopes.yml\n  - conventions/messagebird-conventions.yml\n  - well-known/messagebird-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/authentication/messagebird-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Communications
- Messaging
- SMS
- Email
- WhatsApp
- Voice
- Verification
- CPaaS
- Webhook
- Agents
---
