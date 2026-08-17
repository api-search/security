---
api_key_in:
- header
api_specs:
- filename: postscript-partner-api-openapi.yml
  format: yaml
  label: Postscript Partner API
  slug: postscript-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/_original/postscript-partner-api-openapi.yml
- filename: postscript-subscribers-api-openapi.yml
  format: yaml
  label: Postscript Subscribers API
  slug: postscript-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-subscribers-api-openapi.yml
- filename: postscript-events-api-openapi.yml
  format: yaml
  label: Postscript Events API
  slug: postscript-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-events-api-openapi.yml
- filename: postscript-keywords-api-openapi.yml
  format: yaml
  label: Postscript Keywords API
  slug: postscript-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-keywords-api-openapi.yml
- filename: postscript-messages-api-openapi.yml
  format: yaml
  label: Postscript Messages API
  slug: postscript-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-messages-api-openapi.yml
- filename: postscript-webhooks-api-openapi.yml
  format: yaml
  label: Postscript Webhooks API
  slug: postscript-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-webhooks-api-openapi.yml
- filename: postscript-compliance-api-openapi.yml
  format: yaml
  label: Postscript Compliance API
  slug: postscript-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-compliance-api-openapi.yml
- filename: postscript-identity-api-openapi.yml
  format: yaml
  label: Postscript Identity API
  slug: postscript-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-identity-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Postscript Authentication
name_suffix: Authentication
oauth_flows: []
overview: Postscript secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Postscript
provider_slug: postscript
scheme_count: 2
schemes:
- description: The private API key of the calling identity, sent as a bearer token. Declared as an apiKey scheme with x-bearer-format bearer in Postscript's own published OpenAPI fragments rather than as an http/bearer scheme.
  format: Bearer <private_api_key>
  in: header
  name: sec0
  parameter: Authorization
  sources:
  - openapi/postscript-compliance-api-openapi.yml
  - openapi/postscript-events-api-openapi.yml
  - openapi/postscript-identity-api-openapi.yml
  - openapi/postscript-keywords-api-openapi.yml
  - openapi/postscript-messages-api-openapi.yml
  - openapi/postscript-subscribers-api-openapi.yml
  - openapi/postscript-webhooks-api-openapi.yml
  type: apiKey
- description: Delegation header. A partner acting on behalf of a Shopify shop sends its own partner key in Authorization and that shop's private key here. Shops calling for themselves omit it. It is declared as an operation-level header parameter on all twenty published operations rather than as a securityScheme, so a generic OpenAPI-driven client will not treat it as credential material.
  in: header
  name: X-Postscript-Shop-Token
  parameter: X-Postscript-Shop-Token
  required_for: partners
  sources:
  - openapi/_original/postscript-partner-api-openapi.yml
  type: apiKey
slug: postscript-authentication
source_filename: postscript-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.postscript.io/docs/api-authentication\ndocs: https://developers.postscript.io/docs/api-authentication\nspec_source: openapi/_original/postscript-partner-api-openapi.yml\nprovider: Postscript\napi: Postscript Partner API v2\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oauth: false\n  note: >-\n    Static private API keys only. Postscript operates no OAuth or OpenID Connect surface — every\n    /.well-known/openid-configuration and /.well-known/oauth-authorization-server probe returned 404\n    (postscript.io, developers.postscript.io, app.postscript.io) or 401 (api.postscript.io) on\n    2026-08-13, and no authorization or token endpoint appears anywhere in the documentation. There\n    is therefore no scope model and no scopes/ artifact for this provider.\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer <private_api_key>'\n\
  \  description: >-\n    The private API key of the calling identity, sent as a bearer token. Declared as an apiKey scheme\n    with x-bearer-format bearer in Postscript's own published OpenAPI fragments rather than as an\n    http/bearer scheme.\n  sources:\n  - openapi/postscript-compliance-api-openapi.yml\n  - openapi/postscript-events-api-openapi.yml\n  - openapi/postscript-identity-api-openapi.yml\n  - openapi/postscript-keywords-api-openapi.yml\n  - openapi/postscript-messages-api-openapi.yml\n  - openapi/postscript-subscribers-api-openapi.yml\n  - openapi/postscript-webhooks-api-openapi.yml\n- name: X-Postscript-Shop-Token\n  type: apiKey\n  in: header\n  parameter: X-Postscript-Shop-Token\n  description: >-\n    Delegation header. A partner acting on behalf of a Shopify shop sends its own partner key in\n    Authorization and that shop's private key here. Shops calling for themselves omit it. It is\n    declared as an operation-level header parameter on all twenty published operations\
  \ rather than as\n    a securityScheme, so a generic OpenAPI-driven client will not treat it as credential material.\n  required_for: partners\n  sources:\n  - openapi/_original/postscript-partner-api-openapi.yml\nidentities:\n- role: shop\n  key_type: private API key\n  key_prefix: sk_\n  obtained_from: https://app.postscript.io/account/api\n  note: >-\n    Shops generate a Security Key Pair in the Postscript dashboard. The PUBLIC key (pk_ prefix) is\n    not valid for API authorization — only the private key is.\n- role: partner\n  key_type: private partner API key\n  key_prefix: sk_partner_\n  obtained_from: https://dash.partnerstack.com/application?company=postscript&group=partnerpending\n  note: >-\n    Partner keys are issued by the Postscript team through the partner application, not self-serve.\n    Trigger management needs the partner key alone; anything acting on a shop's data also needs that\n    shop's key in X-Postscript-Shop-Token.\nlegacy:\n  scheme: http basic\n  supported:\
  \ true\n  format: 'Authorization: Basic base64(<private_api_key>:)'\n  note: Username is the private API key, password is empty. Still supported alongside bearer.\nverification_endpoint:\n  operation: verify-identity\n  path: GET /api/v2/me\n  description: Returns the identity a token resolves to, letting a caller confirm which shop or partner it is acting as.\nkey_management:\n  rotation: Shops can regenerate their Security Key Pair from the dashboard.\n  revocation_note: >-\n    Rotating a shop's keys used to invalidate v1 object identifiers, which is why v2 introduced\n    prefixed ids decoupled from the key pair.\n  expiry: none published\n  scopes: none\nsecurity_guidance:\n  from_provider: >-\n    Postscript explicitly warns against calling the API from a browser/front-end because the private\n    key cannot be hidden there, and recommends proxying through your own backend or an intermediary\n    such as Zapier.\n  transport: HTTPS only; api.postscript.io answered TLS 1.3 on probe,\
  \ with no HSTS header set.\naccess_gating:\n  note: >-\n    Since April 2022, custom API access for an individual shop requires an enterprise plan (shops\n    with access before that date are grandfathered). Shops on any plan may still generate keys for\n    use with approved Integration Partners, and Integration Partners keep full API access regardless\n    of the shop's plan.\n  source: https://developers.postscript.io/docs/who-has-access-to-the-partner-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/authentication/postscript-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- SMS
- Marketing
- Messaging
- E-commerce
- Shopify
- RCS
- Subscribers
- Webhooks
- Compliance
---
