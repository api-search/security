---
anonymous_access: false
api_key_in: []
api_specs:
- filename: buymeacoffee-webhooks-openapi.json
  format: json
  label: Buy Me a Coffee Webhooks
  slug: buymeacoffee-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buymeacoffee/openapi/buymeacoffee-webhooks-openapi.json
- filename: buymeacoffee.postman_collection.json
  format: json
  label: Buy Me a Coffee Extras API
  slug: buymeacoffee-extras-api
  spec_type: Postman
  url: https://artifacts.apis.io/buymeacoffee/collections/buymeacoffee.postman_collection.json
- filename: buymeacoffee.postman_collection.json
  format: json
  label: Buy Me a Coffee Subscriptions API
  slug: buymeacoffee-subscriptions-api
  spec_type: Postman
  url: https://artifacts.apis.io/buymeacoffee/collections/buymeacoffee.postman_collection.json
- filename: buymeacoffee.postman_collection.json
  format: json
  label: Buy Me a Coffee Supporters API
  slug: buymeacoffee-supporters-api
  spec_type: Postman
  url: https://artifacts.apis.io/buymeacoffee/collections/buymeacoffee.postman_collection.json
auth_types:
- http
- hmac
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Buy Me a Coffee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buy Me a Coffee secures its APIs with http and hmac across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Buy Me a Coffee
provider_slug: buymeacoffee
scheme_count: 2
schemes:
- description: 'Token-based authentication for the Buy Me a Coffee developer API (https://developers.buymeacoffee.com/api/v1). The developer portal says: "We use token-based authentication... After logging in please generate your token by clicking on the ''generate my token'' button." Tokens are created self-serve in the Developer Dashboard and sent as `Authorization: Bearer <token>`. Read-only and personal (scoped to a single creator''s own account). Browser extensions and client-side JavaScript are explicitly not supported: "the API currently doesn''t support in-browser requests."'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://developers.buymeacoffee.com/#/?id=authentication
  type: http
- algorithm: HMAC-SHA256
  description: Inbound verification scheme for subscribers of Buy Me a Coffee webhooks. The provider POSTs an event envelope and includes `x-signature-sha256` on every request; subscribers compute `HMAC-SHA256(rawBody, signingSecret)` and compare with a constant-time comparison. The signing secret is shown on each webhook detail page in the creator dashboard; rolling the secret immediately invalidates the previous one.
  header: x-signature-sha256
  name: webhookSignature
  sources:
  - https://help.buymeacoffee.com/en/articles/15743173-how-to-setup-and-use-buy-me-a-coffee-webhooks
  - openapi/buymeacoffee-webhooks-openapi.json
  type: hmac
slug: buymeacoffee-authentication
source_filename: buymeacoffee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: searched\nsource:\n- https://developers.buymeacoffee.com/#/?id=authentication\n- https://help.buymeacoffee.com/en/articles/15743173-how-to-setup-and-use-buy-me-a-coffee-webhooks\ndocs: https://developers.buymeacoffee.com/#/?id=authentication\nsummary:\n  types:\n  - http\n  - hmac\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Token-based authentication for the Buy Me a Coffee developer API\n    (https://developers.buymeacoffee.com/api/v1). The developer portal says:\n    \"We use token-based authentication... After logging in please generate\n    your token by clicking on the 'generate my token' button.\" Tokens are\n    created self-serve in the Developer Dashboard and sent as\n    `Authorization: Bearer <token>`. Read-only and personal (scoped to a\n    single creator's own account). Browser extensions and client-side\n    JavaScript are explicitly not supported: \"the API currently doesn't\n    support\
  \ in-browser requests.\"\n  sources:\n  - https://developers.buymeacoffee.com/#/?id=authentication\n- name: webhookSignature\n  type: hmac\n  algorithm: HMAC-SHA256\n  header: x-signature-sha256\n  description: >-\n    Inbound verification scheme for subscribers of Buy Me a Coffee webhooks.\n    The provider POSTs an event envelope and includes `x-signature-sha256`\n    on every request; subscribers compute `HMAC-SHA256(rawBody, signingSecret)`\n    and compare with a constant-time comparison. The signing secret is shown\n    on each webhook detail page in the creator dashboard; rolling the secret\n    immediately invalidates the previous one.\n  sources:\n  - https://help.buymeacoffee.com/en/articles/15743173-how-to-setup-and-use-buy-me-a-coffee-webhooks\n  - openapi/buymeacoffee-webhooks-openapi.json\nnotes: >-\n  The developer API documentation describes the surface as \"Our OAuth API is\n  based around REST\" but publishes only the personal-access-token flow\n  (Bearer). No OAuth authorization-code\
  \ or client-credentials flow is\n  documented in the public portal.\n"
source_yaml_url: https://artifacts.apis.io/buymeacoffee/authentication/buymeacoffee-authentication.yml
summary_line: http/hmac · 2 schemes
tags:
- Creator Economy
- Membership
- Subscription
- Tips
- Payments
- Donations
---
