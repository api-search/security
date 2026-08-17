---
api_key_in:
- header
- cookie
api_specs:
- filename: emotive-open-api-openapi.yml
  format: yaml
  label: Emotive Open API
  slug: emotive-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/openapi/emotive-open-api-openapi.yml
- filename: emotive-subscriber-engine-openapi.yml
  format: yaml
  label: Emotive Lists API (Subscriber Engine)
  slug: emotive-lists-api-subscriber-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/openapi/emotive-subscriber-engine-openapi.yml
- filename: emotive-sensus-webhook-openapi.yml
  format: yaml
  label: Emotive Sensus Webhooks API
  slug: emotive-sensus-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/openapi/emotive-sensus-webhook-openapi.yml
- filename: emotive-helpdesk-openapi.yml
  format: yaml
  label: Emotive Helpdesk API
  slug: emotive-helpdesk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/openapi/emotive-helpdesk-openapi.yml
- filename: emotive-auth-openapi.yml
  format: yaml
  label: Emotive Auth Server API
  slug: emotive-auth-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/openapi/emotive-auth-openapi.yml
- filename: emotive-segments-openapi.yml
  format: yaml
  label: Emotive Segments API
  slug: emotive-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/openapi/emotive-segments-openapi.yml
- filename: emotive-experiences-openapi.yml
  format: yaml
  label: Emotive Experiences API
  slug: emotive-experiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/openapi/emotive-experiences-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Emotive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Emotive secures its APIs with apiKey and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Emotive
provider_slug: emotive
scheme_count: 6
schemes:
- applies_to:
  - Emotive Open API (orders, opt-outs, custom events)
  - Emotive Lists API (subscriber engine)
  - Emotive Sensus Webhooks API (subscriber, profile properties)
  description: Personal access token, scheme-prefixed with the literal word "Token" and a space. Tokens are tied to the brand user account for which they were created. Obtained either by creating a List Growth API signup flow in the app (List Growth -> Integrations -> Add New -> List Growth API), which surfaces a key at the end of the wizard, or by emailing support@emotive.io for an Open API key. There is no self-service developer signup and no key-rotation endpoint.
  docs: https://emotive.gitbook.io/emotive-lists/reference/authentication
  failure_response:
    body: '{"detail": "Authentication credentials were not provided."}'
    observed: 2026-08-13 against https://api.emotiveapp.co/ecommerce/v1/orders/
    status: 401
  format: Token <access_token>
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/emotive-open-api-openapi.yml
  - openapi/emotive-subscriber-engine-openapi.yml
  type: apiKey
- applies_to:
  - Emotive Helpdesk API
  - Emotive Auth Server API
  description: Brand token for the Helpdesk API. Minted by POSTing to /connections/config with an Emotive JWT; each brand may hold only one active token. Used for every subsequent Helpdesk request and for the brand's own webhook configuration.
  docs: https://help.emotive.io/docs/integrations/custom-helpdesk
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/emotive-helpdesk-openapi.yml
  - openapi/emotive-auth-openapi.yml
  type: apiKey
- description: Partner key variant used for the Alloy integration path on the Helpdesk service.
  in: header
  name: AlloyKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/emotive-helpdesk-openapi.yml
  type: apiKey
- description: Internal service-to-service key variant declared on the Helpdesk service.
  in: header
  name: InternalApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/emotive-helpdesk-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: 'Emotive JWT, presented as `Authorization: bearer {emotive JWT}`. Required to bootstrap a Helpdesk brand token and to call the Auth Server''s brand/user management operations.'
  docs: https://help.emotive.io/docs/integrations/custom-helpdesk
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/emotive-helpdesk-openapi.yml
  type: http
- description: Browser session cookie carrying the same Emotive JWT; used by the dashboard.
  in: cookie
  name: cookieAuth
  parameter: access_token_cookie
  sources:
  - openapi/emotive-helpdesk-openapi.yml
  type: apiKey
slug: emotive-authentication
source_filename: emotive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://emotive.gitbook.io/emotive-lists/reference/authentication\ndocs:\n- https://emotive.gitbook.io/emotive-lists/reference/authentication\n- https://help.emotive.io/docs/integrations/custom-site-api\n- https://help.emotive.io/docs/integrations/open-api-integration-orders\n- https://help.emotive.io/docs/integrations/custom-helpdesk\nderived_from:\n- openapi/emotive-auth-openapi.yml\n- openapi/emotive-helpdesk-openapi.yml\n- openapi/emotive-open-api-openapi.yml\n- openapi/emotive-subscriber-engine-openapi.yml\n- openapi/emotive-sensus-webhook-openapi.yml\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header, cookie]\n  oauth2_declared: false\n  openid_connect_declared: false\n  mutual_tls: false\n  note: >-\n    Emotive uses three different credentials on three different surfaces and does not\n    reconcile them anywhere in its documentation. The public Open API and Lists API use\n    a personal access token in an `Authorization:\
  \ Token <token>` header. The API gateway\n    services use an `X-API-Key` header or a bearer JWT. The Auth Server exposes OAuth\n    token endpoints (`POST /oauth/token`, `POST /v2/oauth/token`) plus Auth0, Google and\n    Shopify login legs, but declares no `oauth2` securityScheme and publishes no scope\n    list — the tokens it issues are Emotive session JWTs, not scoped API credentials.\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Token <access_token>'\n  description: >-\n    Personal access token, scheme-prefixed with the literal word \"Token\" and a space.\n    Tokens are tied to the brand user account for which they were created. Obtained\n    either by creating a List Growth API signup flow in the app (List Growth ->\n    Integrations -> Add New -> List Growth API), which surfaces a key at the end of the\n    wizard, or by emailing support@emotive.io for an Open API key. There is no\n    self-service developer signup and no key-rotation\
  \ endpoint.\n  applies_to:\n  - Emotive Open API (orders, opt-outs, custom events)\n  - Emotive Lists API (subscriber engine)\n  - Emotive Sensus Webhooks API (subscriber, profile properties)\n  sources:\n  - openapi/emotive-open-api-openapi.yml\n  - openapi/emotive-subscriber-engine-openapi.yml\n  docs: https://emotive.gitbook.io/emotive-lists/reference/authentication\n  failure_response:\n    status: 401\n    body: '{\"detail\": \"Authentication credentials were not provided.\"}'\n    observed: '2026-08-13 against https://api.emotiveapp.co/ecommerce/v1/orders/'\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: >-\n    Brand token for the Helpdesk API. Minted by POSTing to /connections/config with an\n    Emotive JWT; each brand may hold only one active token. Used for every subsequent\n    Helpdesk request and for the brand's own webhook configuration.\n  applies_to:\n  - Emotive Helpdesk API\n  - Emotive Auth Server API\n  sources:\n  - openapi/emotive-helpdesk-openapi.yml\n\
  \  - openapi/emotive-auth-openapi.yml\n  docs: https://help.emotive.io/docs/integrations/custom-helpdesk\n- name: AlloyKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Partner key variant used for the Alloy integration path on the Helpdesk service.\n  sources: [openapi/emotive-helpdesk-openapi.yml]\n- name: InternalApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Internal service-to-service key variant declared on the Helpdesk service.\n  sources: [openapi/emotive-helpdesk-openapi.yml]\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Emotive JWT, presented as `Authorization: bearer {emotive JWT}`. Required to bootstrap\n    a Helpdesk brand token and to call the Auth Server's brand/user management operations.\n  sources: [openapi/emotive-helpdesk-openapi.yml]\n  docs: https://help.emotive.io/docs/integrations/custom-helpdesk\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter:\
  \ access_token_cookie\n  description: Browser session cookie carrying the same Emotive JWT; used by the dashboard.\n  sources: [openapi/emotive-helpdesk-openapi.yml]\ntoken_endpoints:\n- POST https://api-gw.emotiveapp.co/auth/oauth/token\n- POST https://api-gw.emotiveapp.co/auth/v2/oauth/token\n- POST https://api-gw.emotiveapp.co/auth/auth0/token\n- GET  https://api-gw.emotiveapp.co/auth/google/token\n- GET  https://api-gw.emotiveapp.co/auth/shopify/token\nidentity_providers:\n- Auth0\n- Google\n- Shopify\ngaps:\n- No published OAuth scope list and no oauth2 securityScheme, despite live token endpoints.\n- No self-service API key issuance for the Open API; the docs route developers to support@emotive.io.\n- No documented token rotation, expiry or revocation policy.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emotive/refs/heads/main/authentication/emotive-authentication.yml
summary_line: apiKey/http · 6 schemes
tags:
- Company
- Marketing
- SMS
- Messaging
- eCommerce
- Marketing Automation
- Text Message Marketing
- Conversational Commerce
- Webhooks
- Customer Data
- Segmentation
- Attribution
---
