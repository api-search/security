---
api_key_in:
- basic-auth-username
auth_types:
- http-basic
description: 'Rewardful has three distinct credentials, and they are easy to confuse: a SECRET used for HTTP Basic on the REST API, a PUBLIC key embedded in the browser tracking script, and a per-endpoint webhook Signing Secret. There is no OAuth, no OpenID Connect, no scopes and no per-key permissioning; the REST API Secret is all-or-nothing account access.'
kind: authentication
layout: security
method: searched
name: Rewardful Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rewardful secures its APIs with http-basic across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rewardful
provider_slug: rewardful
scheme_count: 4
schemes:
- credential_location: Rewardful dashboard, Company Settings (https://app.getrewardful.com/company/edit)
  detail: The account API Secret is sent as the HTTP Basic USERNAME with an empty password (`curl https://api.getrewardful.com/v1/affiliates -u YOUR_API_SECRET:`), the same convention Stripe uses. Applied to every documented endpoint.
  name: apiSecretBasic
  privilege: Full account access. The docs state the API Secret "grants full access to your Rewardful account" and must never be shared, committed, emailed, or sent to a browser.
  rotation: No self-service rotation is documented; the docs instruct customers to contact Rewardful support to have a compromised secret rotated.
  scheme: basic
  source: https://developers.rewardful.com/rest-api/overview
  surface: REST API
  type: http
- detail: A PUBLIC key embedded in the `<script async src='https://r.wdfl.co/rw.js' data-rewardful='YOUR-API-KEY'>` tag on the merchant's website. Distinct from the API Secret; it is intended to be visible in page source and only identifies the account for client-side referral attribution and conversion tracking.
  in: html-attribute
  name: trackingApiKey
  parameter_name: data-rewardful
  source: https://developers.rewardful.com/javascript-api/overview
  surface: Browser tracking script
  type: apiKey
- algorithm: HMAC-SHA256
  detail: Each webhook endpoint configured in the dashboard gets its own Signing Secret. Rewardful HMAC-SHA256s the raw request body with that secret and sends the hex digest in the `X-Rewardful-Signature` header. Verification is optional but strongly recommended by the docs.
  name: webhookSigningSecret
  source: https://developers.rewardful.com/webhooks/signed-webhooks
  surface: Outbound webhooks
  type: hmac
- detail: '`GET /v1/affiliates/:id/sso` returns a single-use magic URL that logs an affiliate into their dashboard. Links expire after one minute, cannot be reused, and generating a new one invalidates prior links.'
  name: affiliateMagicLink
  source: https://developers.rewardful.com/rest-api/affiliates/sso
  surface: Affiliate dashboard SSO
  type: bearer-url
slug: rewardful-authentication
source_filename: rewardful-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://developers.rewardful.com/rest-api/overview\ndocs: https://developers.rewardful.com/rest-api/overview\nname: Rewardful Authentication Profile\ndescription: >-\n  Rewardful has three distinct credentials, and they are easy to confuse: a SECRET used for\n  HTTP Basic on the REST API, a PUBLIC key embedded in the browser tracking script, and a\n  per-endpoint webhook Signing Secret. There is no OAuth, no OpenID Connect, no scopes and\n  no per-key permissioning; the REST API Secret is all-or-nothing account access.\nsummary:\n  types: [http-basic]\n  api_key_in: [basic-auth-username]\n  oauth2_flows: []\n  scopes: false\n  mtls: false\n  openid_connect: false\nschemes:\n  - name: apiSecretBasic\n    type: http\n    scheme: basic\n    surface: REST API\n    detail: >-\n      The account API Secret is sent as the HTTP Basic USERNAME with an empty password\n      (`curl https://api.getrewardful.com/v1/affiliates -u YOUR_API_SECRET:`),\
  \ the same\n      convention Stripe uses. Applied to every documented endpoint.\n    credential_location: Rewardful dashboard, Company Settings (https://app.getrewardful.com/company/edit)\n    rotation: >-\n      No self-service rotation is documented; the docs instruct customers to contact\n      Rewardful support to have a compromised secret rotated.\n    privilege: >-\n      Full account access. The docs state the API Secret \"grants full access to your\n      Rewardful account\" and must never be shared, committed, emailed, or sent to a browser.\n    source: https://developers.rewardful.com/rest-api/overview\n  - name: trackingApiKey\n    type: apiKey\n    in: html-attribute\n    parameter_name: data-rewardful\n    surface: Browser tracking script\n    detail: >-\n      A PUBLIC key embedded in the `<script async src='https://r.wdfl.co/rw.js'\n      data-rewardful='YOUR-API-KEY'>` tag on the merchant's website. Distinct from the API\n      Secret; it is intended to be visible in page\
  \ source and only identifies the account\n      for client-side referral attribution and conversion tracking.\n    source: https://developers.rewardful.com/javascript-api/overview\n  - name: webhookSigningSecret\n    type: hmac\n    algorithm: HMAC-SHA256\n    surface: Outbound webhooks\n    detail: >-\n      Each webhook endpoint configured in the dashboard gets its own Signing Secret.\n      Rewardful HMAC-SHA256s the raw request body with that secret and sends the hex digest\n      in the `X-Rewardful-Signature` header. Verification is optional but strongly\n      recommended by the docs.\n    source: https://developers.rewardful.com/webhooks/signed-webhooks\n  - name: affiliateMagicLink\n    type: bearer-url\n    surface: Affiliate dashboard SSO\n    detail: >-\n      `GET /v1/affiliates/:id/sso` returns a single-use magic URL that logs an affiliate into\n      their dashboard. Links expire after one minute, cannot be reused, and generating a new\n      one invalidates prior links.\n\
  \    source: https://developers.rewardful.com/rest-api/affiliates/sso\ntransport:\n  https_required: true\n  note: Webhook receiving endpoints must be served over HTTP/SSL per the webhooks docs.\ngaps:\n  - No OAuth 2.0 or OIDC; third parties cannot obtain delegated, scoped access to a merchant account.\n  - No scopes or read-only keys — every integration holds full-account credentials.\n  - No documented self-service key rotation or multiple concurrent keys.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rewardful/refs/heads/main/authentication/rewardful-authentication.yml
summary_line: http-basic · 4 schemes
tags:
- Affiliate Tracking
- Referral Programs
- Software-as-a-Service
- Stripe
- Commissions
- Payouts
- Affiliate Marketing
- Partner Programs
- Attribution
- Webhook
- Paddle
- Marketing
---
