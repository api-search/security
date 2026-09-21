---
anonymous_access: true
api_key_in: []
api_specs:
- filename: aureliusagent-dev-wundership-mpp-api-openapi.yml
  format: yaml
  label: Wundership MPP API
  slug: wundership-mpp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aureliusagent-dev/refs/heads/main/openapi/aureliusagent-dev-wundership-mpp-api-openapi.yml
- filename: aureliusagent-dev-walton-capacity-mpp-api-openapi.yml
  format: yaml
  label: Walton Capacity MPP API
  slug: walton-capacity-mpp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aureliusagent-dev/refs/heads/main/openapi/aureliusagent-dev-walton-capacity-mpp-api-openapi.yml
auth_types:
- none
- http
description: 'Authentication profile for WunderCorp''s three public surfaces, derived from both OpenAPI documents and upgraded with the provider''s discovery documents and live probes. The defining trait is that there is no credential to obtain in advance: the A2A endpoint is anonymous, the paid REST routes use payment itself as authorization (HTTP 402 challenge, then an MPP credential on retry), and the capacity marketplace issues a per-session access token only after payment. No API key, OAuth 2.0, OpenID Connect or mutual TLS scheme exists anywhere; the "API keys" the 402 body advertises as a human fallback sit behind https://api.wundership.com/api-keys, which answered 403 anonymously.'
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Aureliusagent Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: WunderCorp secures its APIs with none and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WunderCorp
provider_slug: aureliusagent-dev
scheme_count: 5
schemes:
- description: The agent card declares securitySchemes {} and security [] and supportsAuthenticatedExtendedCard false; tasks/get and tasks/cancel answered JSON-RPC responses with no credentials, and agent/getAuthenticatedExtendedCard returns -32601. GET on the endpoint returns 401 with an empty body, which is a method restriction rather than an authentication challenge (no WWW-Authenticate header).
  name: anonymous
  probe:
    credentials: none
    method: POST tasks/get
    status: 200
    url: https://rpc.aureliusagent.dev/a2a
  sources:
  - https://aureliusagent.dev/.well-known/agent-card.json
  surface: Aurelius Agent A2A endpoint https://rpc.aureliusagent.dev/a2a
  type: none
- description: 'Declared in the spec as "MPP payment authorization returned after satisfying the HTTP 402 challenge" and not applied through a security requirement (global security is absent), because the flow is challenge-driven: the unpaid request is answered 402 with WWW-Authenticate: Payment id="<uuid>", realm="mpp.openmodel.sh", method="stripe", intent="charge", request="<base64 {amount,currency}>" (plus Payment-Required: true, X-Wundership-Agent-Payment-Required: true, X-Wundership-Agent-Price and a Link rel="payment"). The client settles the challenge through an MPP client or proxy and "retries the identical request with the MPP Authorization credential" (credentialHeader Authorization, per mpp.json). A verifying proxy may instead present X-Wundership-Agent-Payment-Verified and X-Wundership-Agent-Payment-Receipt (the 402 body''s payment.verifiedHeader / receiptHeader; the provider''s argent CLI adds X-Wundership-Agent-Payment-Secret for operator-side verification). Success returns
    paymentVerified true, a receipt, and on the capacity API a Payment-Receipt header. Payment rail: Stripe Shared Payment Token (card, Link), networkId published in mpp.json and the spec''s x-machine-payment-rails.'
  name: mppPayment
  probe:
    method: POST (unpaid)
    realm: mpp.openmodel.sh
    status: 402
    url: https://mpp.openmodel.sh/v1/plan
    www_authenticate_scheme: Payment
  scheme: Payment
  sources:
  - openapi/aureliusagent-dev-wundership-mpp-api-openapi.yml
  - https://mpp.openmodel.sh/.well-known/mpp.json
  surface: Wundership MPP API paid routes (postWundershipPlan, postBuilderPreview, postImageGeneration, postListingFromImage, postOpenmodelPricingEstimate and the deprecated /mpp/* routes) and Walton POST /mpp/capacity/sessions
  type: http
- description: 'GET /v1/capabilities: "gatewayApiKeyRequired: false"; "The upstream provider HTTP 402 status and WWW-Authenticate challenge are passed through unchanged"; "The caller retries the same OpenModel gateway URL with the MPP Authorization credential"; "Upstream Authentication-Info and payment receipt headers are passed through unchanged". The gateway therefore holds no credential of its own; the upstream model provider is the relying party. Observed: unpaid POST /v1/chat/completions returned 402 application/problem+json.'
  name: upstreamMppPassthrough
  probe:
    content_type: application/problem+json
    method: POST (unpaid)
    status: 402
    url: https://mpp.openmodel.sh/v1/chat/completions
  scheme: Payment (upstream provider's)
  sources:
  - https://mpp.openmodel.sh/v1/capabilities
  surface: OpenModel MPP inference gateway (postMppChatCompletions, postMppResponses, postMppMessages, postMppEmbeddings, postMppImageGeneration, postMppAudioTranscription, postMppAudioSpeech, postMppModeration, relayMppProviderRequest)
  type: http
- description: Not declared as a securityScheme; modelled in the spec as a required header parameter on each session route and returned as a response header (and CapacitySession.accessToken) from the paid 201 of POST /mpp/capacity/sessions. mpp.json names it capacity.accessHeader and marks those routes payment mode "already_paid" with authorization.header X-Capacity-Access-Token. A per-session capability token issued by payment, not an account key.
  in: header
  name: X-Capacity-Access-Token
  sources:
  - openapi/aureliusagent-dev-walton-capacity-mpp-api-openapi.yml
  - https://mpp.openmodel.sh/.well-known/mpp.json
  surface: Walton Capacity MPP API session routes (GET /mpp/capacity/sessions/{sessionId}, POST .../peering-profile, .../connection-confirmed, .../cancel)
  type: apiKey
- description: Declared securityScheme applied to the two capacity-PROVIDER operations (listing an asset, publishing a peering handoff). mpp.json labels the peering-offer route "authenticated provider". How a provider obtains the bearer token is not documented publicly.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/aureliusagent-dev-walton-capacity-mpp-api-openapi.yml
  surface: Walton Capacity MPP API provider-side routes (POST /capacity/assets, POST /capacity/sessions/{sessionId}/peering-offer)
  type: http
slug: aureliusagent-dev-authentication
source_filename: aureliusagent-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource:\n- openapi/aureliusagent-dev-wundership-mpp-api-openapi.yml (securitySchemes.mppPayment)\n- openapi/aureliusagent-dev-walton-capacity-mpp-api-openapi.yml (securitySchemes.bearerAuth; X-Capacity-Access-Token header parameter and 201 response header)\n- https://mpp.openmodel.sh/.well-known/mpp.json (capacity.accessHeader, endpoints[].payment credentialHeader/challengeHeader/receiptHeader)\n- https://mpp.openmodel.sh/v1/capabilities (paymentBehavior, gatewayApiKeyRequired)\n- https://aureliusagent.dev/.well-known/agent-card.json (securitySchemes {}, security [])\n- live unpaid POST https://mpp.openmodel.sh/v1/plan (402 challenge) and JSON-RPC probes of https://rpc.aureliusagent.dev/a2a (2026-09-19)\ndocs: https://wundercorp.co/agents/\ndescription: >-\n  Authentication profile for WunderCorp's three public surfaces, derived from both OpenAPI documents and\n  upgraded with the provider's discovery documents and live probes. The\
  \ defining trait is that there is no\n  credential to obtain in advance: the A2A endpoint is anonymous, the paid REST routes use payment itself\n  as authorization (HTTP 402 challenge, then an MPP credential on retry), and the capacity marketplace\n  issues a per-session access token only after payment. No API key, OAuth 2.0, OpenID Connect or mutual\n  TLS scheme exists anywhere; the \"API keys\" the 402 body advertises as a human fallback sit behind\n  https://api.wundership.com/api-keys, which answered 403 anonymously.\nsummary:\n  types: [none, http]\nschemes:\n- name: anonymous\n  type: none\n  surface: Aurelius Agent A2A endpoint https://rpc.aureliusagent.dev/a2a\n  description: >-\n    The agent card declares securitySchemes {} and security [] and supportsAuthenticatedExtendedCard false;\n    tasks/get and tasks/cancel answered JSON-RPC responses with no credentials, and\n    agent/getAuthenticatedExtendedCard returns -32601. GET on the endpoint returns 401 with an empty body,\n\
  \    which is a method restriction rather than an authentication challenge (no WWW-Authenticate header).\n  sources: [https://aureliusagent.dev/.well-known/agent-card.json]\n  probe: {url: 'https://rpc.aureliusagent.dev/a2a', method: 'POST tasks/get', status: 200, credentials: none}\n- name: mppPayment\n  type: http\n  scheme: Payment\n  surface: Wundership MPP API paid routes (postWundershipPlan, postBuilderPreview, postImageGeneration, postListingFromImage, postOpenmodelPricingEstimate and the deprecated /mpp/* routes) and Walton POST /mpp/capacity/sessions\n  description: >-\n    Declared in the spec as \"MPP payment authorization returned after satisfying the HTTP 402 challenge\"\n    and not applied through a security requirement (global security is absent), because the flow is\n    challenge-driven: the unpaid request is answered 402 with WWW-Authenticate: Payment id=\"<uuid>\",\n    realm=\"mpp.openmodel.sh\", method=\"stripe\", intent=\"charge\", request=\"<base64 {amount,currency}>\"\
  \ (plus\n    Payment-Required: true, X-Wundership-Agent-Payment-Required: true, X-Wundership-Agent-Price and a Link\n    rel=\"payment\"). The client settles the challenge through an MPP client or proxy and \"retries the\n    identical request with the MPP Authorization credential\" (credentialHeader Authorization, per\n    mpp.json). A verifying proxy may instead present X-Wundership-Agent-Payment-Verified and\n    X-Wundership-Agent-Payment-Receipt (the 402 body's payment.verifiedHeader / receiptHeader; the\n    provider's argent CLI adds X-Wundership-Agent-Payment-Secret for operator-side verification). Success\n    returns paymentVerified true, a receipt, and on the capacity API a Payment-Receipt header. Payment\n    rail: Stripe Shared Payment Token (card, Link), networkId published in mpp.json and the spec's\n    x-machine-payment-rails.\n  sources:\n  - openapi/aureliusagent-dev-wundership-mpp-api-openapi.yml\n  - https://mpp.openmodel.sh/.well-known/mpp.json\n  probe: {url: 'https://mpp.openmodel.sh/v1/plan',\
  \ method: 'POST (unpaid)', status: 402, www_authenticate_scheme: Payment, realm: mpp.openmodel.sh}\n- name: upstreamMppPassthrough\n  type: http\n  scheme: Payment (upstream provider's)\n  surface: OpenModel MPP inference gateway (postMppChatCompletions, postMppResponses, postMppMessages, postMppEmbeddings, postMppImageGeneration, postMppAudioTranscription, postMppAudioSpeech, postMppModeration, relayMppProviderRequest)\n  description: >-\n    GET /v1/capabilities: \"gatewayApiKeyRequired: false\"; \"The upstream provider HTTP 402 status and\n    WWW-Authenticate challenge are passed through unchanged\"; \"The caller retries the same OpenModel\n    gateway URL with the MPP Authorization credential\"; \"Upstream Authentication-Info and payment receipt\n    headers are passed through unchanged\". The gateway therefore holds no credential of its own; the\n    upstream model provider is the relying party. Observed: unpaid POST /v1/chat/completions returned 402\n    application/problem+json.\n\
  \  sources: [https://mpp.openmodel.sh/v1/capabilities]\n  probe: {url: 'https://mpp.openmodel.sh/v1/chat/completions', method: 'POST (unpaid)', status: 402, content_type: application/problem+json}\n- name: X-Capacity-Access-Token\n  type: apiKey\n  in: header\n  surface: Walton Capacity MPP API session routes (GET /mpp/capacity/sessions/{sessionId}, POST .../peering-profile, .../connection-confirmed, .../cancel)\n  description: >-\n    Not declared as a securityScheme; modelled in the spec as a required header parameter on each session\n    route and returned as a response header (and CapacitySession.accessToken) from the paid 201 of POST\n    /mpp/capacity/sessions. mpp.json names it capacity.accessHeader and marks those routes payment mode\n    \"already_paid\" with authorization.header X-Capacity-Access-Token. A per-session capability token\n    issued by payment, not an account key.\n  sources:\n  - openapi/aureliusagent-dev-walton-capacity-mpp-api-openapi.yml\n  - https://mpp.openmodel.sh/.well-known/mpp.json\n\
  - name: bearerAuth\n  type: http\n  scheme: bearer\n  surface: Walton Capacity MPP API provider-side routes (POST /capacity/assets, POST /capacity/sessions/{sessionId}/peering-offer)\n  description: >-\n    Declared securityScheme applied to the two capacity-PROVIDER operations (listing an asset, publishing a\n    peering handoff). mpp.json labels the peering-offer route \"authenticated provider\". How a provider\n    obtains the bearer token is not documented publicly.\n  sources: [openapi/aureliusagent-dev-walton-capacity-mpp-api-openapi.yml]\noauth: false\nopenid_connect: false\napi_keys: false\napi_keys_note: >-\n  The 402 body's humanFallback points at https://api.wundership.com/api-keys (\"Subscribe for persistent API\n  keys, higher quotas, deployment access, managed BuilderStudio resources, and usage-based billing\"); it\n  returned 403 {\"error\":\"Origin is not allowed.\"} on 2026-09-19 and no key format, header name or scope\n  model is published, so no key scheme is recorded.\n\
  notes: >-\n  /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource and\n  /.well-known/openid-configuration are absent on every host (well-known/aureliusagent-dev-well-known.yml);\n  no scopes/ artifact is written because there is no scope surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aureliusagent-dev/refs/heads/main/authentication/aureliusagent-dev-authentication.yml
summary_line: none/http · 5 schemes
tags:
- Company
- Agents
- A2A
- Machine Payments
- MPP
- HTTP 402
- Artificial Intelligence
- Inference Gateway
- Code Generation
- Developer Tools
- Compute Capacity
- Orchestration
---
