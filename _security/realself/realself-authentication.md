---
api_key_in: []
api_specs:
- filename: realself-lead-sharing-asyncapi.yml
  format: yaml
  label: RealSelf Lead Sharing
  slug: realself-lead-sharing
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/realself/refs/heads/main/asyncapi/realself-lead-sharing-asyncapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Realself Authentication
name_suffix: Authentication
oauth_flows: []
overview: RealSelf declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: RealSelf
provider_slug: realself
scheme_count: 2
schemes:
- applies_to: inbound Lead Sharing notifications (RealSelf -> partner endpoint)
  description: Every SNS message carries Signature, SignatureVersion and SigningCertURL. RealSelf's own example validates with the AWS SDK before processing and returns 401 Unauthorized on failure. This is the only authentication on the inbound leg — there is no shared secret, bearer token or mTLS between RealSelf and the partner endpoint.
  evidence: https://github.com/RealSelf/rs-lead-sharing-subscriber-example#processing-notification
  headers:
  - x-amz-sns-message-type
  - x-amz-sns-message-id
  - x-amz-sns-topic-arn
  - x-amz-sns-subscription-arn
  id: sns-message-signature
  transport: https POST from "Amazon Simple Notification Service Agent"
  type: message-signature
  verification: Amazon.SimpleNotificationService.Util.Message.IsMessageSignatureValid()
- algorithm: ES512
  applies_to: outbound lead-update callback (partner -> RealSelf)
  claims:
  - lead_id
  - exp
  description: Each notification carries a `callback` URL and a `token`. The token is a detached-style JWS whose header declares alg ES512, typ JOSE+JSON, a kid, and a jku pointing at a JWKS document; its payload carries `lead_id` and an `exp`. The token is also appended to the callback URL as a `token` query parameter in RealSelf's published example.
  evidence: json-schema/realself-new-lead-webhook-1-0-0.json (properties.token)
  expiry: short-lived (exp claim present in the published example token)
  id: lead-callback-jws
  jwks:
    jku_observed: https://api.rsdev.co/.well-known/jwks.json
    note: The jku in RealSelf's published example points at their DEVELOPMENT host (api.rsdev.co). Neither that URL nor https://api.realself.com/.well-known/jwks.json is anonymously readable — both return 403 Missing Authentication Token — so key material cannot be verified from outside an onboarded partner account.
  token_location: query parameter `token` on the callback URL, and the `token` payload field
  type: jws-token
slug: realself-authentication
source_filename: realself-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://github.com/RealSelf/rs-lead-sharing-subscriber-example (RealSelf's published\n  subscriber reference implementation) and\n  https://api.realself.com/v1/schemas/leads/new-lead-webhook/1-0-0.json\nsummary: >-\n  RealSelf publishes no public developer program, no API key issuance flow and no OAuth\n  surface. The one documented integration — Lead Sharing — uses two distinct, non-interactive\n  credentials, neither of which a developer requests self-service: inbound messages are\n  authenticated by the Amazon SNS message signature, and the callback that lets a partner\n  post updates back is authorised by a short-lived JWS token RealSelf mints per lead.\n  Everything else on api.realself.com is closed: any unmatched route answers HTTP 403\n  {\"message\":\"Missing Authentication Token\"} (an AWS API Gateway route miss).\nschemes:\n- id: sns-message-signature\n  type: message-signature\n  applies_to: inbound Lead Sharing\
  \ notifications (RealSelf -> partner endpoint)\n  transport: https POST from \"Amazon Simple Notification Service Agent\"\n  description: >-\n    Every SNS message carries Signature, SignatureVersion and SigningCertURL. RealSelf's own\n    example validates with the AWS SDK before processing and returns 401 Unauthorized on\n    failure. This is the only authentication on the inbound leg — there is no shared secret,\n    bearer token or mTLS between RealSelf and the partner endpoint.\n  headers:\n  - x-amz-sns-message-type\n  - x-amz-sns-message-id\n  - x-amz-sns-topic-arn\n  - x-amz-sns-subscription-arn\n  verification: Amazon.SimpleNotificationService.Util.Message.IsMessageSignatureValid()\n  evidence: https://github.com/RealSelf/rs-lead-sharing-subscriber-example#processing-notification\n- id: lead-callback-jws\n  type: jws-token\n  applies_to: outbound lead-update callback (partner -> RealSelf)\n  description: >-\n    Each notification carries a `callback` URL and a `token`. The token\
  \ is a detached-style\n    JWS whose header declares alg ES512, typ JOSE+JSON, a kid, and a jku pointing at a JWKS\n    document; its payload carries `lead_id` and an `exp`. The token is also appended to the\n    callback URL as a `token` query parameter in RealSelf's published example.\n  algorithm: ES512\n  token_location: query parameter `token` on the callback URL, and the `token` payload field\n  claims:\n  - lead_id\n  - exp\n  jwks:\n    jku_observed: https://api.rsdev.co/.well-known/jwks.json\n    note: >-\n      The jku in RealSelf's published example points at their DEVELOPMENT host (api.rsdev.co).\n      Neither that URL nor https://api.realself.com/.well-known/jwks.json is anonymously\n      readable — both return 403 Missing Authentication Token — so key material cannot be\n      verified from outside an onboarded partner account.\n  expiry: short-lived (exp claim present in the published example token)\n  evidence: json-schema/realself-new-lead-webhook-1-0-0.json (properties.token)\n\
  onboarding:\n  self_service: false\n  model: >-\n    Partner onboarding is sales-mediated. RealSelf provisions the SNS topic and subscribes the\n    partner's endpoint; there is no developer signup, key dashboard or public request flow.\n  contact: https://www.realself.com/dr/advertise\noauth2: false\nopenid_connect: false\napi_keys: false\nmutual_tls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realself/refs/heads/main/authentication/realself-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Healthcare
- Aesthetics
- Marketplace
- Reviews
- Lead Generation
- Consumer Health
- Webhook
- JSON-Schema
---
