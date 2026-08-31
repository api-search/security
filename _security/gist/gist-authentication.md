---
api_key_in:
- header
api_specs:
- filename: gist-chat-api-openapi.yml
  format: yaml
  label: Gist Chat API
  slug: gist-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gist/refs/heads/main/openapi/gist-chat-api-openapi.yml
- filename: gist-health-api-openapi.yml
  format: yaml
  label: Gist Health API
  slug: gist-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gist/refs/heads/main/openapi/gist-health-api-openapi.yml
- filename: gist-publishers-api-openapi.yml
  format: yaml
  label: Gist Publishers API
  slug: gist-publishers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gist/refs/heads/main/openapi/gist-publishers-api-openapi.yml
- filename: gist-questions-api-openapi.yml
  format: yaml
  label: Gist Questions API
  slug: gist-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gist/refs/heads/main/openapi/gist-questions-api-openapi.yml
- filename: gist-root-api-openapi.yml
  format: yaml
  label: Gist Root API
  slug: gist-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gist/refs/heads/main/openapi/gist-root-api-openapi.yml
- filename: gist-summaries-api-openapi.yml
  format: yaml
  label: Gist Summaries API
  slug: gist-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gist/refs/heads/main/openapi/gist-summaries-api-openapi.yml
- filename: gist-threads-api-openapi.yml
  format: yaml
  label: Gist Threads API
  slug: gist-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gist/refs/heads/main/openapi/gist-threads-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Gist Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gist secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gist
provider_slug: gist
scheme_count: 1
schemes:
- applies_to: 14 of the 16 operations. GET /v1/health and GET / declare no security and are documented as public endpoints; GET /v1/health was verified anonymously on 2026-08-12 and returned 200.
  description: Add your API key with the Bearer prefix (e.g., "Bearer YOUR-API-KEY")
  format: Bearer <api-key>
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/gist-answers-api-openapi.yml
  type: apiKey
slug: gist-authentication
source_filename: gist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/gist-answers-api-openapi.yml\ndocs: https://platform.gist.ai/docs/gist-content-api\nnote: >-\n  Derived from the harvested OpenAPI securityScheme, then upgraded from the developer hub, which\n  documents key issuance, the tenancy header and the two additional credential shapes the spec\n  does not cover (the widget attributes and the ad-tag publisher pair). Gist has no OAuth surface\n  at all — no oauth2 scheme in the spec, no OAuth docs, and /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server 404 on every host — so no scopes/ artifact is emitted.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer <api-key>'\n  description: Add your API key with the Bearer prefix (e.g., \"Bearer YOUR-API-KEY\")\n  sources: [openapi/gist-answers-api-openapi.yml]\n\
  \  applies_to: >-\n    14 of the 16 operations. GET /v1/health and GET / declare no security and are documented as\n    public endpoints; GET /v1/health was verified anonymously on 2026-08-12 and returned 200.\nkey_issuance:\n  level: Publisher Group\n  self_serve: false\n  quote: >-\n    \"A unique API key is issued at the Publisher Group level for authentication. API keys are\n    provided during onboarding. Contact us if you need access.\"\n  source: https://platform.gist.ai/docs/gist-content-api\n  note: >-\n    One key covers every publication inside a Publisher Group, which makes the key the tenancy\n    boundary as well as the credential. No key prefix convention, rotation policy or expiry is\n    published.\ntenancy:\n  header: X-User-ID\n  required: true\n  value: the caller's domain or organization identifier\n  applies_to: Chat, Threads, Questions and Publishers operations\n  note: >-\n    Carried alongside the API key rather than derived from it, and identical to the `user-id`\n\
  \    attribute publishers set on the gist-chat-widget / gist-search-widget elements.\nother_credential_surfaces:\n- surface: Gist Answers web components\n  credentials: [api-key, user-id]\n  transport: HTML attributes on the custom element, visible in page source\n  source: https://platform.gist.ai/docs/quick-start-using-widgets\n  note: >-\n    The widget key is embedded client-side, so it is necessarily a public/publishable credential.\n    The docs do not distinguish a public key from a secret key, though the API reference for\n    POST /v1/summaries does say the endpoint \"requires a valid API key (public or secret)\" —\n    implying a two-key model that is never documented.\n- surface: Gist Ads ad tag and native SDKs\n  credentials: [publisherID, publisherKey]\n  transport: >-\n    `window.prtag.defineSlot({id, api_key, url, geo}, ...)` in the browser; publisherID and\n    publisherKey parameters on GistAdControl in the iOS and Android SDKs. The search ad service at\n    tp-srch-api.prorata.ai\
  \ answers every unauthenticated request with 401\n    \"Publisher-ID and Publisher-Key required\", so those are the header names.\n  source: https://github.com/Prorata-ai/PrtAdsSDK\ngaps:\n- No documented key rotation, expiry or revocation.\n- No documented distinction between the public and secret key hinted at in the summaries reference.\n- No scopes or permissions model; a Publisher Group key is all-or-nothing across its publications.\n- No OAuth 2.0, OIDC or mTLS option for enterprise publishers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gist/refs/heads/main/authentication/gist-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Generative AI
- Advertising
- Marketing
- Brand Visibility
- Publishers
- Search
- Content
- Answer Engine
- Attribution
- Content Licensing
- Media
- RAG
- Advertising Technology
---
