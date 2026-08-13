---
api_key_in: []
auth_types:
- none
- session
description: ''
kind: authentication
layout: security
method: probed
name: Black Crow Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Black Crow AI secures its APIs with none and session across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Black Crow AI
provider_slug: black-crow-ai
scheme_count: 3
schemes:
- applies_to: POST https://api.blackcrow.ai/v1/events/{event_name}
  description: 'The event ingest endpoint accepts anonymous cross-origin requests. A POST with an empty JSON body was answered 400 with field-validation errors (siteName / pageId / visitorId must not be null) — never 401 or 403 — so no credential is required to reach validation. CORS is fully open: Access-Control-Allow-Origin "*", Access-Control-Allow-Methods "GET, POST, PUT", Access-Control-Allow-Headers "Content-Type" (no Authorization header is permitted through preflight, which confirms no bearer scheme is in use).'
  evidence:
  - fetched: '2026-08-12'
    http_status: 400
    method: POST
    url: https://api.blackcrow.ai/v1/events/view
  - fetched: '2026-08-12'
    http_status: 200
    method: OPTIONS
    url: https://api.blackcrow.ai/v1/events/view
  identity_carried_in:
  - field: siteName
    in: body
    note: customer/site identifier; the tag derives it from the bundle filename (xyz.js -> "xyz") or from Shopify.shop
  - field: visitorId
    in: body
    note: first-party visitor identifier, persisted in the _bcai_z cookie (set browser-side, or at the edge by @bcai/edge-sdk)
  - field: pageId
    in: body
  name: unauthenticated-tag-ingest
  type: none
- applies_to: https://app.blackcrow.ai/
  description: 'The Black Crow Portal (settings, product toggles, dashboards, Predictive Offer and Enhanced CAPI controls) is behind an interactive sign-in at https://app.blackcrow.ai/sign-in. No OpenID Connect or OAuth discovery document is served: /.well-known/openid-configuration and /.well-known/oauth-authorization-server returned 404 on both app.blackcrow.ai and api.blackcrow.ai on 2026-08-12.'
  evidence:
  - fetched: '2026-08-12'
    http_status: 404
    url: https://app.blackcrow.ai/.well-known/openid-configuration
  - fetched: '2026-08-12'
    http_status: 404
    url: https://api.blackcrow.ai/.well-known/oauth-authorization-server
  name: portal-session
  type: session
- applies_to: customer marketing platforms (Klaviyo, Attentive, Postscript, Sendlane, Mailchimp, Alia, Justuno, Meta, Google Ads, TikTok, Shopify)
  description: Black Crow does not issue credentials; it CONSUMES them. Onboarding is a sequence of granting Black Crow access to the customer's own marketing platforms (help center "Step 2 - Connect your platforms", plus one "Platform Access" article per platform), and installing the Shopify app. The credential model is therefore inbound-delegated, not outbound-issued.
  docs: https://blackcrow.zendesk.com/hc/en-us/articles/20768291848475-Step-2-Connect-your-platforms
  name: platform-oauth-delegation
  type: delegated
slug: black-crow-ai-authentication
source_filename: black-crow-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  Live probes of https://api.blackcrow.ai/v1/events/* (2026-08-12) plus the first-party\n  browser bundle https://init.blackcrow.ai/js/core/example.js (HTTP 200) and the Black Crow AI\n  help center article \"JavaScript\"\n  (https://blackcrow.zendesk.com/hc/en-us/articles/20203743583387-JavaScript).\ndocs: https://blackcrow.zendesk.com/hc/en-us/articles/20203743583387-JavaScript\nnote: >-\n  Black Crow AI publishes no OpenAPI, so no securitySchemes could be derived. This profile is\n  built from what the ingest endpoint actually accepts and from how the provider's own tag\n  authenticates itself. There is NO developer-facing API key programme: access to the platform\n  is provisioned by Black Crow (a Customer Success Manager enables features), and the browser\n  tag is identified by site rather than by a secret.\nsummary:\n  types: [none, session]\n  api_key_in: []\n  oauth2_flows: []\n  developer_credentials_issued: false\n\
  schemes:\n- name: unauthenticated-tag-ingest\n  type: none\n  applies_to: POST https://api.blackcrow.ai/v1/events/{event_name}\n  description: >-\n    The event ingest endpoint accepts anonymous cross-origin requests. A POST with an empty\n    JSON body was answered 400 with field-validation errors (siteName / pageId / visitorId\n    must not be null) — never 401 or 403 — so no credential is required to reach validation.\n    CORS is fully open: Access-Control-Allow-Origin \"*\", Access-Control-Allow-Methods\n    \"GET, POST, PUT\", Access-Control-Allow-Headers \"Content-Type\" (no Authorization header\n    is permitted through preflight, which confirms no bearer scheme is in use).\n  identity_carried_in:\n  - {field: siteName, in: body, note: 'customer/site identifier; the tag derives it from the bundle filename (xyz.js -> \"xyz\") or from Shopify.shop'}\n  - {field: visitorId, in: body, note: 'first-party visitor identifier, persisted in the _bcai_z cookie (set browser-side, or at the\
  \ edge by @bcai/edge-sdk)'}\n  - {field: pageId, in: body}\n  evidence:\n  - {url: 'https://api.blackcrow.ai/v1/events/view', method: POST, http_status: 400, fetched: '2026-08-12'}\n  - {url: 'https://api.blackcrow.ai/v1/events/view', method: OPTIONS, http_status: 200, fetched: '2026-08-12'}\n- name: portal-session\n  type: session\n  applies_to: https://app.blackcrow.ai/\n  description: >-\n    The Black Crow Portal (settings, product toggles, dashboards, Predictive Offer and\n    Enhanced CAPI controls) is behind an interactive sign-in at\n    https://app.blackcrow.ai/sign-in. No OpenID Connect or OAuth discovery document is\n    served: /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n    returned 404 on both app.blackcrow.ai and api.blackcrow.ai on 2026-08-12.\n  evidence:\n  - {url: 'https://app.blackcrow.ai/.well-known/openid-configuration', http_status: 404, fetched: '2026-08-12'}\n  - {url: 'https://api.blackcrow.ai/.well-known/oauth-authorization-server',\
  \ http_status: 404, fetched: '2026-08-12'}\n- name: platform-oauth-delegation\n  type: delegated\n  applies_to: customer marketing platforms (Klaviyo, Attentive, Postscript, Sendlane, Mailchimp, Alia, Justuno, Meta, Google Ads, TikTok, Shopify)\n  description: >-\n    Black Crow does not issue credentials; it CONSUMES them. Onboarding is a sequence of\n    granting Black Crow access to the customer's own marketing platforms (help center\n    \"Step 2 - Connect your platforms\", plus one \"Platform Access\" article per platform),\n    and installing the Shopify app. The credential model is therefore inbound-delegated,\n    not outbound-issued.\n  docs: https://blackcrow.zendesk.com/hc/en-us/articles/20768291848475-Step-2-Connect-your-platforms\ngaps:\n- No public API key, token, or OAuth client registration exists for third-party developers.\n- No .well-known/oauth-protected-resource, no scopes surface — scopes/ is correctly absent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-crow-ai/refs/heads/main/authentication/black-crow-ai-authentication.yml
summary_line: none/session · 3 schemes
tags:
- Company
- Ecommerce
- Artificial Intelligence
- Machine Learning
- Marketing
- Advertising
- Personalization
- Conversion Optimization
- Analytics
- Event Ingest
- Tag Management
- Shopify
---
