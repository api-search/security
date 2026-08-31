---
api_key_in: []
api_specs:
- filename: useapi-account-api-openapi.yml
  format: yaml
  label: useapi.net Account API
  slug: useapi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useapi/refs/heads/main/openapi/useapi-account-api-openapi.yml
- filename: useapi-dreamina-api-openapi.yml
  format: yaml
  label: useapi.net Dreamina API
  slug: useapi-dreamina-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useapi/refs/heads/main/openapi/useapi-dreamina-api-openapi.yml
- filename: useapi-faceswap-api-openapi.yml
  format: yaml
  label: useapi.net Faceswap API
  slug: useapi-faceswap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useapi/refs/heads/main/openapi/useapi-faceswap-api-openapi.yml
- filename: useapi-flowmusic-api-openapi.yml
  format: yaml
  label: useapi.net Flowmusic API
  slug: useapi-flowmusic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useapi/refs/heads/main/openapi/useapi-flowmusic-api-openapi.yml
- filename: useapi-google-flow-api-openapi.yml
  format: yaml
  label: useapi.net Google Flow API
  slug: useapi-google-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useapi/refs/heads/main/openapi/useapi-google-flow-api-openapi.yml
- filename: useapi-jobs-api-openapi.yml
  format: yaml
  label: useapi.net Jobs API
  slug: useapi-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useapi/refs/heads/main/openapi/useapi-jobs-api-openapi.yml
- filename: useapi-kling-api-openapi.yml
  format: yaml
  label: useapi.net Kling API
  slug: useapi-kling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useapi/refs/heads/main/openapi/useapi-kling-api-openapi.yml
- filename: useapi-minimax-api-openapi.yml
  format: yaml
  label: useapi.net Minimax API
  slug: useapi-minimax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useapi/refs/heads/main/openapi/useapi-minimax-api-openapi.yml
- filename: useapi-mureka-api-openapi.yml
  format: yaml
  label: useapi.net Mureka API
  slug: useapi-mureka-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useapi/refs/heads/main/openapi/useapi-mureka-api-openapi.yml
- filename: useapi-pixverse-api-openapi.yml
  format: yaml
  label: useapi.net Pixverse API
  slug: useapi-pixverse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useapi/refs/heads/main/openapi/useapi-pixverse-api-openapi.yml
- filename: useapi-runwayml-api-openapi.yml
  format: yaml
  label: useapi.net Runwayml API
  slug: useapi-runwayml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useapi/refs/heads/main/openapi/useapi-runwayml-api-openapi.yml
- filename: useapi-tempolor-api-openapi.yml
  format: yaml
  label: useapi.net Tempolor API
  slug: useapi-tempolor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useapi/refs/heads/main/openapi/useapi-tempolor-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Useapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: useapi.net secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: useapi.net
provider_slug: useapi
scheme_count: 1
schemes:
- applies_to: all twelve captured APIs, all 298 operations
  description: The useapi.net subscription token. Emailed to the subscriber on signup and retrieved from the setup page. No expiry or rotation mechanism is documented.
  example_shape: user:12345-abcdefghi
  format: Bearer user:<number>-<unique-string>
  header: Authorization
  name: bearerAuth
  rules:
  - Use the complete token string, including the `user:` prefix and the alphanumeric suffix.
  - Do not truncate to just the numeric portion.
  - Do not URL-encode the token.
  scheme: bearer
  sources:
  - openapi/useapi-dreamina-v1-openapi.yml
  - openapi/useapi-faceswap-v1-openapi.yml
  - openapi/useapi-flowmusic-v1-openapi.yml
  - openapi/useapi-google-flow-v1-openapi.yml
  - openapi/useapi-kling-v1-openapi.yml
  - openapi/useapi-midjourney-v1-openapi.yml
  - openapi/useapi-midjourney-v2-openapi.yml
  - openapi/useapi-minimax-v1-openapi.yml
  - openapi/useapi-mureka-v1-openapi.yml
  - openapi/useapi-pixverse-v2-openapi.yml
  - openapi/useapi-runwayml-v1-openapi.yml
  - openapi/useapi-tempolor-v1-openapi.yml
  type: http
slug: useapi-authentication
source_filename: useapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource:\n- https://useapi.net/llms.txt\n- https://useapi.net/docs/start-here/setup-useapi\n- https://useapi.net/docs/account-management\n- openapi/ (securitySchemes derived from the first-party Postman collections)\ndocs: https://useapi.net/docs/start-here/setup-useapi\n\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  oauth2_flows: []\n  api_key_in: []\n  model: single long-lived platform bearer token, no scopes\n  note: >-\n    One token authorizes every useapi.net API on the subscription. There is no OAuth, no OpenID\n    Connect, no per-API key, no scope system, and no documented rotation or revocation endpoint.\n    /.well-known/openid-configuration and /.well-known/oauth-authorization-server both return 404.\n\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Bearer user:<number>-<unique-string>'\n  example_shape: 'user:12345-abcdefghi'\n  description: >-\n    The useapi.net\
  \ subscription token. Emailed to the subscriber on signup and retrieved from the\n    setup page. No expiry or rotation mechanism is documented.\n  rules:\n  - Use the complete token string, including the `user:` prefix and the alphanumeric suffix.\n  - Do not truncate to just the numeric portion.\n  - Do not URL-encode the token.\n  applies_to: all twelve captured APIs, all 298 operations\n  sources:\n  - openapi/useapi-dreamina-v1-openapi.yml\n  - openapi/useapi-faceswap-v1-openapi.yml\n  - openapi/useapi-flowmusic-v1-openapi.yml\n  - openapi/useapi-google-flow-v1-openapi.yml\n  - openapi/useapi-kling-v1-openapi.yml\n  - openapi/useapi-midjourney-v1-openapi.yml\n  - openapi/useapi-midjourney-v2-openapi.yml\n  - openapi/useapi-minimax-v1-openapi.yml\n  - openapi/useapi-mureka-v1-openapi.yml\n  - openapi/useapi-pixverse-v2-openapi.yml\n  - openapi/useapi-runwayml-v1-openapi.yml\n  - openapi/useapi-tempolor-v1-openapi.yml\n\nsecond_factor_credentials:\n  description: >-\n    Platform authentication\
  \ is only half the story. Because useapi.net is a bring-your-own-account\n    fronting layer, calling a generation endpoint also requires credentials for the caller's own\n    account on the wrapped AI service, registered ahead of time through that service's\n    POST /accounts endpoint. These are session-grade secrets, not API keys.\n  credential_types:\n  - service: google-flow\n    credential: cookies copied from accounts.google.com\n    registered_via: POST /v1/google-flow/accounts\n    selector: email\n  - service: flowmusic\n    credential: Google sign-in session / refresh token\n    registered_via: POST /v1/flowmusic/accounts\n    selector: email\n  - service: dreamina, kling, minimax, mureka, pixverse, runwayml, tempolor\n    credential: site session cookies or account credentials\n    registered_via: POST /v1/<service>/accounts\n    selector: account (email on runwayml and flowmusic)\n  - service: faceswap\n    credential: Discord token + server id + channel id\n    registered_via:\
  \ POST /v1/faceswap/account/{channel_id}\n    selector: channel_id\n  security_implication: >-\n    Handing full browser session cookies for a third-party consumer account to an intermediary is a\n    material trust decision, and the vendor's own Q&A acknowledges that automating these accounts\n    runs against the wrapped services' terms of use. Assess this before adoption; it is the defining\n    risk of the platform, not an incidental detail.\n\nfailure_modes:\n- status: 401\n  meaning: Missing, malformed or invalid useapi.net token.\n  body: '{\"error\": \"Unauthorized\"}'\n- status: 402\n  meaning: Token is valid but the useapi.net subscription is expired.\n  body: '{\"error\": \"Account has no subscription or subscription expired\"}'\n- status: 403\n  meaning: Token is valid but the referenced resource belongs to a different useapi.net user.\n  body: '{\"error\": \"Unauthorized access to user:12345 detected in character reference\"}'\n- status: 596\n  meaning: >-\n    Non-standard\
  \ status. The useapi.net token is fine but the linked upstream account's session or\n    refresh token was rejected. Delete and re-register that account.\n  body: '{\"error\": \"Account user@email.com in error state: refresh token rejected\", \"code\": 596}'\n\nrelated:\n  scopes: none — no OAuth scope surface exists, so no scopes/ artifact is emitted\n  conventions: conventions/useapi-conventions.yml\n  errors: errors/useapi-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/useapi/refs/heads/main/authentication/useapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Generative AI
- Video Generation
- Image-Generation
- Music Generation
- Text-to-Speech
- Face Swap
- API Aggregator
- Machine-Learning
- Media
- Webhook
---
