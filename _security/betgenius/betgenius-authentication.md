---
api_key_in:
- header
api_specs:
- filename: betgenius-booking-v2-openapi.yml
  format: yaml
  label: BetGenius Booking API V2
  slug: betgenius-booking-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/openapi/betgenius-booking-v2-openapi.yml
- filename: betgenius-booking-v1-openapi.yml
  format: yaml
  label: BetGenius Booking API V1
  slug: betgenius-booking-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/openapi/betgenius-booking-v1-openapi.yml
- filename: betgenius-video-v3-openapi.yml
  format: yaml
  label: BetGenius Video Streaming API v3
  slug: betgenius-video-streaming-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/openapi/betgenius-video-v3-openapi.yml
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Betgenius Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: BetGenius secures its APIs with http, apiKey, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: BetGenius
provider_slug: betgenius
scheme_count: 5
schemes:
- applies_to: Booking API (V1 and V2)
  description: Basic HTTP Authentication. "To access the Booking API, our Support team will provide you with the exclusive Username and Password." Credentials are formatted {UserName}:{Password}.
  docs: https://geniussports.atlassian.net/wiki/spaces/BID/pages/36084721/Booking+API
  name: basic
  scheme: basic
  sources:
  - openapi/betgenius-booking-v1-openapi.yml
  - openapi/betgenius-booking-v2-openapi.yml
  type: http
- applies_to: Video Streaming API v3
  description: 'AWS Cognito user-pool authorizer fronted by API Gateway (x-amazon-apigateway-authtype: cognito_user_pools). The bearer value goes in the Authorization header.'
  in: header
  name: CognitoPool
  parameter: Authorization
  sources:
  - openapi/betgenius-video-v3-openapi.yml
  type: apiKey
- applies_to: Video Streaming API v3, Match State Platform APIs, Statistics API
  description: Issued API key. Per the platform auth docs, "An issued API Key controls the available quotas, rate limits, and throttling." Required alongside the bearer token on every request.
  in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/betgenius-video-v3-openapi.yml
  type: apiKey
- description: OAuth2 client_credentials against an Amazon Cognito issuer (cognito-idp.eu-west-1.amazonaws.com). The access token is passed in an AUTHORIZATION header and must be paired with the x-api-key header. This scheme is documented in the BetGenius Integration Documents and governs the Match State Platform, Access Control, Schedule and Statistics APIs used by the sportsbook live-data integration; it is not declared in the three OpenAPI files harvested into openapi/, which cover Booking and Video only.
  docs: https://geniussports.atlassian.net/wiki/spaces/BID/pages/3925901961/Match+State+Platform+APIs+Authentication
  flow: clientCredentials
  method: searched
  name: OAuth2
  token_lifetime_seconds: 3600
  token_type: Bearer
  token_urls:
    production: https://auth.api.geniussports.com/oauth2/token
    uat: https://uat.auth.api.geniussports.com/oauth2/token
  type: oauth2
- algorithm: HMAC-SHA256
  applies_to: Genius Live Player widgetLoader, BetVision
  description: 'The embeddable Genius Live Player / BetVision widget is authorised per end user, not per integrator: the `digest` query parameter is "an HMAC-SHA256 hash of the end user''s device ID (MAID) and a shared secret", with the shared secret issued by the Genius onboarding team. Region/DMA entitlement is enforced at the edge — an out-of-market viewer never receives the player_ready event.'
  docs: https://dap-docs.betstream.betgenius.com/video-player/web-browser-integration
  method: searched
  name: HMAC digest (Genius Live Player)
  type: signature
slug: betgenius-authentication
source_filename: betgenius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/betgenius-booking-v1-openapi.yml, openapi/betgenius-booking-v2-openapi.yml, openapi/betgenius-video-v3-openapi.yml\ndocs:\n  - https://geniussports.atlassian.net/wiki/spaces/BID/pages/3925901961/Match+State+Platform+APIs+Authentication\n  - https://geniussports.atlassian.net/wiki/spaces/BID/pages/36084721/Booking+API\n  - https://geniussports.atlassian.net/wiki/spaces/BID/pages/6779994181/Secure+sign-in+for+Data+Services+two-step+verification\nnote: >-\n  BetGenius runs three different auth models across three product surfaces, and an integrator has\n  to implement all three. Nothing is self-service: every credential on this platform is issued by\n  a Genius Sports integration manager or the Support team to a contracted sportsbook.\nsummary:\n  types: [http, apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  self_service: false\n  credential_issuance: manual — issued by the Genius Sports\
  \ integration/onboarding team\nschemes:\n  - name: basic\n    type: http\n    scheme: basic\n    description: >-\n      Basic HTTP Authentication. \"To access the Booking API, our Support team will provide you with\n      the exclusive Username and Password.\" Credentials are formatted {UserName}:{Password}.\n    applies_to: Booking API (V1 and V2)\n    sources:\n      - openapi/betgenius-booking-v1-openapi.yml\n      - openapi/betgenius-booking-v2-openapi.yml\n    docs: https://geniussports.atlassian.net/wiki/spaces/BID/pages/36084721/Booking+API\n  - name: CognitoPool\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: >-\n      AWS Cognito user-pool authorizer fronted by API Gateway\n      (x-amazon-apigateway-authtype: cognito_user_pools). The bearer value goes in the\n      Authorization header.\n    applies_to: Video Streaming API v3\n    sources: [openapi/betgenius-video-v3-openapi.yml]\n  - name: api_key\n    type: apiKey\n    in: header\n    parameter:\
  \ x-api-key\n    description: >-\n      Issued API key. Per the platform auth docs, \"An issued API Key controls the available quotas,\n      rate limits, and throttling.\" Required alongside the bearer token on every request.\n    applies_to: Video Streaming API v3, Match State Platform APIs, Statistics API\n    sources: [openapi/betgenius-video-v3-openapi.yml]\n  - name: OAuth2\n    type: oauth2\n    flow: clientCredentials\n    token_urls:\n      production: https://auth.api.geniussports.com/oauth2/token\n      uat: https://uat.auth.api.geniussports.com/oauth2/token\n    token_lifetime_seconds: 3600\n    token_type: Bearer\n    description: >-\n      OAuth2 client_credentials against an Amazon Cognito issuer\n      (cognito-idp.eu-west-1.amazonaws.com). The access token is passed in an AUTHORIZATION header\n      and must be paired with the x-api-key header. This scheme is documented in the BetGenius\n      Integration Documents and governs the Match State Platform, Access Control,\
  \ Schedule and\n      Statistics APIs used by the sportsbook live-data integration; it is not declared in the three\n      OpenAPI files harvested into openapi/, which cover Booking and Video only.\n    docs: https://geniussports.atlassian.net/wiki/spaces/BID/pages/3925901961/Match+State+Platform+APIs+Authentication\n    method: searched\n  - name: HMAC digest (Genius Live Player)\n    type: signature\n    algorithm: HMAC-SHA256\n    description: >-\n      The embeddable Genius Live Player / BetVision widget is authorised per end user, not per\n      integrator: the `digest` query parameter is \"an HMAC-SHA256 hash of the end user's device ID\n      (MAID) and a shared secret\", with the shared secret issued by the Genius onboarding team.\n      Region/DMA entitlement is enforced at the edge — an out-of-market viewer never receives the\n      player_ready event.\n    applies_to: Genius Live Player widgetLoader, BetVision\n    docs: https://dap-docs.betstream.betgenius.com/video-player/web-browser-integration\n\
  \    method: searched\nportal_authentication:\n  surface: Data Services web portal (InPlay Manager, PreMatch Manager, Event Viewer)\n  model: password + emailed magic link (two-step verification)\n  note: >-\n    Explicitly NOT an authenticator app, SMS code, or hardware key — \"Today the second step is\n    email only.\" Rolled out incrementally per customer organisation.\n  docs: https://geniussports.atlassian.net/wiki/spaces/BID/pages/6779994181/Secure+sign-in+for+Data+Services+two-step+verification\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/authentication/betgenius-authentication.yml
summary_line: http/apiKey/oauth2 · 5 schemes
tags:
- Sportsbook
- Sports Betting
- Sports Data
- Odds Feeds
- Trading Services
- Risk Management
- Live Streaming
- In-Play Betting
- BetBuilder
- Player Engagement
- Marketing Technology
- Gambling
---
