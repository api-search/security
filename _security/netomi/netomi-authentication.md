---
api_key_in: []
api_specs:
- filename: netomi-agentdesk-openapi.json
  format: json
  label: Netomi Platform API
  slug: netomi-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netomi/refs/heads/main/openapi/netomi-agentdesk-openapi.json
auth_types:
- bearer-jwt
- tenant-identifier
description: ''
kind: authentication
layout: security
method: searched
name: Netomi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Netomi secures its APIs with bearer-jwt and tenant-identifier across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Netomi
provider_slug: netomi
scheme_count: 4
schemes:
- description: The Netomi bot reference ID issued per enterprise account. Passed to NetomiChat.shared.initialize(botRefId:env:) on iOS and NCWChatSdk.initialize(..., newBotRefId = ...) on Android. It selects the tenant/bot, not the user; it is not a secret credential on its own.
  in: sdk-initialization
  name: botRefId
  required: true
  source: SDK docs (installation.md, usage.md)
  type: tenantIdentifier
- description: Selects the Netomi regional backend the SDK talks to. iOS enum NCWEnvironment (parameter `env`); Android NCWEnvironment. The flag isDynamicEnv is set true only when the bot is configured for dynamic SDK configuration.
  in: sdk-initialization
  name: environment
  required: true
  source: https://github.com/msgai/netomi-chat-ios/blob/main/docs/usage.md
  type: regionSelector
  values:
  - USProd
  - EUProd
  - SGProd
  - QA
  - QAInternal
  - Development
- bearerFormat: JWT
  description: A JSON Web Token supplied by the integrating application when the bot is configured for authenticated sessions. Passed at launch — launch(jwt:), launchWithQuery(_:jwt:), launchAsync(jwt:) — and again on reauthorization. When a bot does not require authentication the SDK runs an anonymous guest session and a supplied JWT is safely ignored. There is no separate login endpoint.
  guidance: Netomi documents JWTs as short-lived credentials that must be generated server-side, scoped to the user, and refreshed via the reauthorization flow rather than embedded as long-lived tokens in the app.
  name: jwt
  required: conditional
  scheme: bearer
  source: https://github.com/msgai/netomi-chat-ios/blob/main/docs/events-and-auth.md
  type: http
- description: Arbitrary HTTP headers attached to every SDK API request via updateApiHeaderConfiguration(headers:). Documented for app version, device id, platform, user segment, experiment variant and locale (X-App-Version, X-Device-ID, X-Platform, X-User-Type, X-Experiment-Variant, X-Locale in the published example). Netomi explicitly warns against placing long-lived secrets here.
  in: header
  name: custom API headers
  required: false
  source: https://github.com/msgai/netomi-chat-ios/blob/main/docs/advanced.md
  type: apiKey
slug: netomi-authentication
source_filename: netomi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://github.com/msgai/netomi-chat-ios/blob/main/docs/events-and-auth.md\ndocs:\n- https://github.com/msgai/netomi-chat-ios/blob/main/docs/events-and-auth.md\n- https://github.com/msgai/netomi-chat-android-app/blob/main/docs/events-and-auth.md\n- https://github.com/msgai/netomi-chat-ios/blob/main/docs/security-and-privacy.md\nnote: |\n  Netomi's live AgentDesk OpenAPI 3.1.0 (https://api.netomi.com/v3/api-docs) declares\n  ZERO securitySchemes across all 67 operations, so\n  0-working/derive-authentication.py produced no profile from it — the contract is\n  silent about credentials. This profile is therefore searched from the first-party\n  Mobile Chat SDK documentation and supplemented with the credential-shaped surfaces\n  that ARE visible in the spec (the visitor authorization request body and the two\n  named headers on the platform status operation). The server-to-server / Agentic\n  Studio credential model remains undocumented\
  \ publicly (docs.netomi.com is\n  login-gated).\nsummary:\n  types: [bearer-jwt, tenant-identifier]\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  spec_declared_security_schemes: 0\n  openid_connect: false\n  mutual_tls: false\n  public_spec: true\n  public_spec_source: https://api.netomi.com/v3/api-docs\nschemes:\n- name: botRefId\n  type: tenantIdentifier\n  in: sdk-initialization\n  required: true\n  description: The Netomi bot reference ID issued per enterprise account. Passed to\n    NetomiChat.shared.initialize(botRefId:env:) on iOS and NCWChatSdk.initialize(...,\n    newBotRefId = ...) on Android. It selects the tenant/bot, not the user; it is not\n    a secret credential on its own.\n  source: SDK docs (installation.md, usage.md)\n- name: environment\n  type: regionSelector\n  in: sdk-initialization\n  required: true\n  values: [USProd, EUProd, SGProd, QA, QAInternal, Development]\n  description: Selects the Netomi regional backend the SDK talks to. iOS enum\n    NCWEnvironment\
  \ (parameter `env`); Android NCWEnvironment. The flag isDynamicEnv\n    is set true only when the bot is configured for dynamic SDK configuration.\n  source: https://github.com/msgai/netomi-chat-ios/blob/main/docs/usage.md\n- name: jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  required: conditional\n  description: A JSON Web Token supplied by the integrating application when the bot\n    is configured for authenticated sessions. Passed at launch — launch(jwt:),\n    launchWithQuery(_:jwt:), launchAsync(jwt:) — and again on reauthorization. When\n    a bot does not require authentication the SDK runs an anonymous guest session and\n    a supplied JWT is safely ignored. There is no separate login endpoint.\n  guidance: Netomi documents JWTs as short-lived credentials that must be generated\n    server-side, scoped to the user, and refreshed via the reauthorization flow rather\n    than embedded as long-lived tokens in the app.\n  source: https://github.com/msgai/netomi-chat-ios/blob/main/docs/events-and-auth.md\n\
  - name: custom API headers\n  type: apiKey\n  in: header\n  required: false\n  description: Arbitrary HTTP headers attached to every SDK API request via\n    updateApiHeaderConfiguration(headers:). Documented for app version, device id,\n    platform, user segment, experiment variant and locale (X-App-Version, X-Device-ID,\n    X-Platform, X-User-Type, X-Experiment-Variant, X-Locale in the published example).\n    Netomi explicitly warns against placing long-lived secrets here.\n  source: https://github.com/msgai/netomi-chat-ios/blob/main/docs/advanced.md\nsessions:\n  models:\n  - name: guest\n    default: true\n    description: Anonymous, SDK-managed session. No JWT required.\n  - name: authenticated\n    description: Identity established by the JWT for a bot configured to require one.\n  reauthorization:\n    flow: The SDK emits a `reauthorizationRequest` event; the host app re-authenticates\n      the user and answers with sendEventToSdk(type:.reauthorizationSuccess, jwt:) —\n    \
  \  a fresh JWT is REQUIRED on success — or .reauthorizationFailure.\n    logout: clearChatSession() ends the active conversation, dismisses the chat UI and\n      clears stored session state before launching as a different user.\n  identity_metadata:\n    api: setCustomParameter([String:String]) / sendCustomParameter(name:value:)\n    note: Custom parameters are metadata forwarded to the AI backend for personalisation.\n      Netomi documents them explicitly as NOT credentials and NOT an authentication\n      mechanism.\nspec_observed:\n  note: Credential-bearing surfaces visible in openapi/netomi-agentdesk-openapi.json\n    even though no securityScheme is declared.\n  surfaces:\n  - name: ExternalAuthenticationRequest\n    used_by: messagesPost_4 (POST /v1/authorize/visitors)\n    fields: [authToken, clientId, authCode, visitorKey, timestamp, expiryTime]\n    description: Exchange an externally issued token or auth code for an authorized\n      Netomi visitor. This is the server-side\
  \ counterpart of the SDK's JWT session.\n  - name: X-Hub-Signature\n    in: header\n    required: true\n    used_by: statusAPI (GET /v1/platform/status)\n    description: HMAC-style request signature header. Only operation in the spec that\n      declares it; the signing algorithm and secret provisioning are not documented.\n  - name: X-Client-Id\n    in: header\n    required: true\n    used_by: statusAPI (GET /v1/platform/status)\n    description: Client identifier paired with X-Hub-Signature.\n  - name: secretId\n    in: path\n    used_by: healthCheck (GET /ceaas/v1/health/{secretId})\n    description: Opaque secret embedded in the health-check path.\n  - name: oAuthRedirect\n    used_by: oAuthRedirect (GET /v1/oauth/redirect)\n    description: An OAuth redirect handler exists for outbound integrations, but no\n      OAuth authorization server, token endpoint, scopes or flows are declared for the\n      Netomi API itself. No scopes/ artifact was emitted.\ngaps:\n- The public OpenAPI\
  \ declares no securitySchemes at all, so there is nothing\n  machine-readable for a client to negotiate against.\n- No OAuth 2.0 or OpenID Connect surface published; /.well-known/openid-configuration\n  and /.well-known/oauth-authorization-server return 404 on every Netomi host.\n- No public documentation of the server-to-server Platform API credential model\n  (docs.netomi.com is login-gated).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netomi/refs/heads/main/authentication/netomi-authentication.yml
summary_line: bearer-jwt/tenant-identifier · 4 schemes
tags:
- Company
- Artificial Intelligence
- Agentic AI
- Customer Experience
- Customer Service
- Customer-Support
- Conversational AI
- Chatbots
- Chat
- Voice
- Telephony
- SDK
- Mobile
---
