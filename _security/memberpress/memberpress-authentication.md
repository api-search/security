---
api_key_in:
- header
api_specs:
- filename: memberpress-developer-tools-openapi.yml
  format: yaml
  label: MemberPress Developer Tools REST API
  slug: developer-tools-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/openapi/memberpress-developer-tools-openapi.yml
auth_types:
- apiKey
- wordpress-capability
description: ''
kind: authentication
layout: security
method: searched
name: Memberpress Authentication
name_suffix: Authentication
oauth_flows: []
overview: MemberPress secures its APIs with apiKey and wordpress-capability across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MemberPress
provider_slug: memberpress
scheme_count: 3
schemes:
- description: Developer Tools API key. Generated automatically when the Developer Tools add-on is activated and regenerable from the MemberPress > Developer screen if compromised. This is the header name MemberPress documents on its own docs site.
  in: header
  issuance: Self-service inside WP Admin (MemberPress > Developer). No vendor approval step.
  name: MemberPressApiKey
  parameter: MEMBERPRESS-API-KEY
  rotation: Regenerate from the Developer screen. MemberPress documents regeneration as the remedy for a compromised key; there is no published overlap/grace window.
  source: https://memberpress.com/docs/overview-of-using-the-developer-tools/
  type: apiKey
- description: The same Developer Tools API key sent in the `Authorization` header. This is the form used throughout the MemberPress REST API documentation repository and in every request of its published Postman collection. It is a BARE key, not an RFC 7235 `Bearer <token>` credential — an agent that prefixes `Bearer ` will fail.
  in: header
  name: AuthorizationApiKey
  parameter: Authorization
  source: https://github.com/caseproof/memberpress-rest-api-documentation#authentication
  type: apiKey
- description: A logged-in WordPress user holding the `remove_users` capability (typically an administrator) is authorized without an API key. Callers lacking the capability receive HTTP 401.
  in: cookie
  name: WordPressUserCapability
  parameter: wordpress_logged_in_*
  source: https://github.com/caseproof/memberpress-rest-api-documentation#authentication
  type: session
slug: memberpress-authentication
source_filename: memberpress-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://memberpress.com/docs/overview-of-using-the-developer-tools/\ndocs:\n- https://memberpress.com/docs/overview-of-using-the-developer-tools/\n- https://github.com/caseproof/memberpress-rest-api-documentation#authentication\n- https://memberpress.com/docs/developer-tools-actions/\nsummary:\n  types:\n  - apiKey\n  - wordpress-capability\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  note: >-\n    MemberPress is self-hosted. Credentials are issued by the MemberPress Developer Tools add-on\n    inside the customer's own WordPress installation — there is no vendor-operated identity\n    provider, no OAuth authorization server and no token exchange. MemberPress publishes two\n    different header names for the same key across its own documentation surfaces; both are\n    recorded below rather than picking one.\nschemes:\n- name: MemberPressApiKey\n  type: apiKey\n  in: header\n  parameter:\
  \ MEMBERPRESS-API-KEY\n  description: >-\n    Developer Tools API key. Generated automatically when the Developer Tools add-on is activated\n    and regenerable from the MemberPress > Developer screen if compromised. This is the header\n    name MemberPress documents on its own docs site.\n  issuance: Self-service inside WP Admin (MemberPress > Developer). No vendor approval step.\n  rotation: Regenerate from the Developer screen. MemberPress documents regeneration as the\n    remedy for a compromised key; there is no published overlap/grace window.\n  source: https://memberpress.com/docs/overview-of-using-the-developer-tools/\n- name: AuthorizationApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    The same Developer Tools API key sent in the `Authorization` header. This is the form used\n    throughout the MemberPress REST API documentation repository and in every request of its\n    published Postman collection. It is a BARE key, not an RFC 7235\
  \ `Bearer <token>` credential —\n    an agent that prefixes `Bearer ` will fail.\n  source: https://github.com/caseproof/memberpress-rest-api-documentation#authentication\n- name: WordPressUserCapability\n  type: session\n  in: cookie\n  parameter: wordpress_logged_in_*\n  description: >-\n    A logged-in WordPress user holding the `remove_users` capability (typically an administrator)\n    is authorized without an API key. Callers lacking the capability receive HTTP 401.\n  source: https://github.com/caseproof/memberpress-rest-api-documentation#authentication\nwebhook_authentication:\n- name: MemberPressWebhookKey\n  in: header\n  parameter: memberpress-webhook-key\n  direction: inbound-to-subscriber\n  description: >-\n    Webhook Key introduced in MemberPress 1.2.5. MemberPress sends this header on outbound webhook\n    deliveries so the receiving endpoint can verify the call. This is a shared secret, not an HMAC\n    signature over the payload — a receiver cannot verify body integrity,\
  \ only origin possession\n    of the key.\n  source: https://memberpress.com/docs/overview-of-using-the-developer-tools/\n- name: BasicAuthentication\n  in: header\n  parameter: Authorization\n  description: >-\n    MemberPress additionally documents Basic Authentication (with the WordPress Application\n    Passwords plugin) for webhook delivery, describing it in its own documentation as the \"less\n    secure\" option.\n  source: https://memberpress.com/docs/overview-of-using-the-developer-tools/\ngaps:\n- No OAuth 2.0 or OpenID Connect surface — key-auth only, so there is no scope model and no\n  scopes/ artifact for this provider.\n- No published key-expiry, key-scoping or per-key permission model. A Developer Tools key is\n  effectively administrator-equivalent over every MemberPress resource.\n- Webhook deliveries carry a static shared secret rather than a per-payload signature.\n- The `/me/permissions` endpoint that would let a caller discover its own authorization is\n  documented\
  \ by MemberPress as not present in all installations.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memberpress/refs/heads/main/authentication/memberpress-authentication.yml
summary_line: apiKey/wordpress-capability · 3 schemes
tags:
- Company
- Membership
- Subscriptions
- WordPress
- Payments
- E-Commerce
- Courses
- Content Management
- Webhooks
- MCP
---
