---
api_key_in: []
api_specs:
- filename: squarespace-orders-api-openapi.yml
  format: yaml
  label: Squarespace Orders API
  slug: squarespace-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-orders-api-openapi.yml
- filename: squarespace-products-api-openapi.yml
  format: yaml
  label: Squarespace Products API
  slug: squarespace-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-products-api-openapi.yml
- filename: squarespace-inventory-api-openapi.yml
  format: yaml
  label: Squarespace Inventory API
  slug: squarespace-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-inventory-api-openapi.yml
- filename: squarespace-profiles-api-openapi.yml
  format: yaml
  label: Squarespace Profiles API
  slug: squarespace-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-profiles-api-openapi.yml
- filename: squarespace-transactions-api-openapi.yml
  format: yaml
  label: Squarespace Transactions API
  slug: squarespace-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-transactions-api-openapi.yml
- filename: squarespace-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Squarespace Webhook Subscriptions API
  slug: squarespace-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-webhook-subscriptions-api-openapi.yml
- filename: squarespace-site-api-openapi.yml
  format: yaml
  label: Squarespace Site API
  slug: squarespace-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-site-api-openapi.yml
- filename: squarespace-commerce-api-v2-openapi.json
  format: json
  label: Squarespace Commerce API
  slug: squarespace-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-commerce-api-v2-openapi.json
auth_types:
- http
- oauth2
description: 'Squarespace Commerce APIs accept two credential types over one wire format. Every request carries `Authorization: Bearer <token>`, where the token is either a merchant-generated API key or an OAuth 2.0 access token. The published OpenAPI collapses both into a single `http bearer` scheme named `Authorization`, so the machine-readable contract cannot distinguish them — the split is documented only in prose, and it matters, because several behaviours differ by credential type (the Create Order rate limit, and the OAuth-only Webhook Subscriptions API).'
kind: authentication
layout: security
method: searched
name: Squarespace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Squarespace secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Squarespace
provider_slug: squarespace
scheme_count: 2
schemes:
- description: API key or OAuth access token. Documented header default in the reference is "Bearer YOUR_API_KEY_OR_OAUTH_TOKEN".
  name: Authorization
  scheme: bearer
  sources:
  - openapi/squarespace-commerce-api-v2-openapi.json
  - openapi/squarespace-inventory-api-openapi.yml
  - openapi/squarespace-orders-api-openapi.yml
  - openapi/squarespace-products-api-openapi.yml
  - openapi/squarespace-profiles-api-openapi.yml
  - openapi/squarespace-site-api-openapi.yml
  - openapi/squarespace-transactions-api-openapi.yml
  - openapi/squarespace-webhook-subscriptions-api-openapi.yml
  type: http
- authorizationUrl: https://login.squarespace.com/api/1/login/oauth/provider/authorize
  declared_in_openapi: false
  description: OAuth 2.0 authorization code grant used by Squarespace Extensions. Client registration is manual and reviewed by Squarespace — there is no dynamic client registration and no self-service credential issuance for new clients beyond the registration form.
  flow: authorizationCode
  name: oauth2
  scopes_artifact: scopes/squarespace-scopes.yml
  sources:
  - https://developers.squarespace.com/oauth
  tokenUrl: https://login.squarespace.com/api/1/login/oauth/provider/tokens
  type: oauth2
slug: squarespace-authentication
source_filename: squarespace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.squarespace.com/commerce-apis/authentication-and-permissions\ndocs: https://developers.squarespace.com/commerce-apis/authentication-and-permissions\nderived_from:\n  - openapi/squarespace-commerce-api-v2-openapi.json\n  - openapi/squarespace-inventory-api-openapi.yml\n  - openapi/squarespace-orders-api-openapi.yml\n  - openapi/squarespace-products-api-openapi.yml\n  - openapi/squarespace-profiles-api-openapi.yml\n  - openapi/squarespace-site-api-openapi.yml\n  - openapi/squarespace-transactions-api-openapi.yml\n  - openapi/squarespace-webhook-subscriptions-api-openapi.yml\ndescription: >-\n  Squarespace Commerce APIs accept two credential types over one wire format. Every request carries\n  `Authorization: Bearer <token>`, where the token is either a merchant-generated API key or an\n  OAuth 2.0 access token. The published OpenAPI collapses both into a single `http bearer` scheme\n  named `Authorization`,\
  \ so the machine-readable contract cannot distinguish them — the split is\n  documented only in prose, and it matters, because several behaviours differ by credential type\n  (the Create Order rate limit, and the OAuth-only Webhook Subscriptions API).\nsummary:\n  types:\n    - http\n    - oauth2\n  machine_readable_types:\n    - http\n  note: >-\n    oauth2 is fully documented but NOT declared in the OpenAPI. A tool reading only the spec will\n    conclude Squarespace is bearer-token-only and will miss the entire Extensions/OAuth path.\nschemes:\n  - name: Authorization\n    type: http\n    scheme: bearer\n    description: >-\n      API key or OAuth access token. Documented header default in the reference is\n      \"Bearer YOUR_API_KEY_OR_OAUTH_TOKEN\".\n    sources:\n      - openapi/squarespace-commerce-api-v2-openapi.json\n      - openapi/squarespace-inventory-api-openapi.yml\n      - openapi/squarespace-orders-api-openapi.yml\n      - openapi/squarespace-products-api-openapi.yml\n\
  \      - openapi/squarespace-profiles-api-openapi.yml\n      - openapi/squarespace-site-api-openapi.yml\n      - openapi/squarespace-transactions-api-openapi.yml\n      - openapi/squarespace-webhook-subscriptions-api-openapi.yml\n  - name: oauth2\n    type: oauth2\n    flow: authorizationCode\n    declared_in_openapi: false\n    authorizationUrl: https://login.squarespace.com/api/1/login/oauth/provider/authorize\n    tokenUrl: https://login.squarespace.com/api/1/login/oauth/provider/tokens\n    scopes_artifact: scopes/squarespace-scopes.yml\n    description: >-\n      OAuth 2.0 authorization code grant used by Squarespace Extensions. Client registration is\n      manual and reviewed by Squarespace — there is no dynamic client registration and no\n      self-service credential issuance for new clients beyond the registration form.\n    sources:\n      - https://developers.squarespace.com/oauth\ncredentials:\n  - kind: api-key\n    name: Developer API Key\n    issuance: >-\n      Self-service\
  \ in the Squarespace admin: Settings > Advanced > Developer API Keys > GENERATE KEY.\n      Requires the Squarespace Advanced (Commerce Advanced) plan.\n    transport: Authorization Bearer header\n    permission_model: >-\n      Permission level (Read Only / Read and Write) selected per Commerce API at generation time.\n      Permissions on an issued key CANNOT be modified — a new key must be generated.\n    expiry: >-\n      Keys never expire as long as the merchant site remains active. There is no documented rotation\n      mechanism and no expiry-based forcing function.\n    visibility: Shown once at generation; not retrievable afterwards.\n    restrictions:\n      - Not available for the Webhook Subscriptions API (OAuth only).\n      - Subject to the stricter 100/hour Create Order limit that OAuth callers are exempt from.\n    source: https://developers.squarespace.com/commerce-apis/authentication-and-permissions\n  - kind: oauth-token\n    name: OAuth 2.0 access token\n    issuance:\
  \ >-\n      Authorization code grant after manual Squarespace review and issuance of client_id/client_secret.\n    transport: Authorization Bearer header\n    access_token_ttl: 30m\n    refresh: grant_type=refresh_token, requires access_type=offline on the authorize call\n    token_endpoint_auth: >-\n      HTTP Basic — the client builds an Authorization header from its OAuth 2.0 credentials.\n    permission_model: Comma-separated website.* scopes; see scopes/squarespace-scopes.yml\n    restrictions:\n      - Permissions cannot be changed on an existing grant; the merchant must re-initiate the connection.\n    source: https://developers.squarespace.com/oauth\ntransport_requirements:\n  - requirement: HTTPS only\n    detail: All requests sent over HTTP instead of HTTPS are rejected.\n  - requirement: User-Agent required\n    detail: Requests without a User-Agent header are rejected; default client User-Agents may be rate-limited harder.\n  - requirement: No CORS\n    detail: >-\n      Squarespace\
  \ explicitly does not support browser-side calls and documents CORS as a security\n      risk because it would expose the bearer token; a server-side proxy is the documented pattern.\n    source: https://developers.squarespace.com/commerce-apis/faq\nwebhook_authentication:\n  mechanism: HMAC-SHA256 request signature\n  header: Squarespace-Signature\n  secret: >-\n    Returned only when creating a subscription or rotating a secret; a rotateSecret operation exists\n    (POST /1.0/webhook_subscriptions/{subscriptionId}/actions/rotateSecret).\n  source: https://developers.squarespace.com/webhooks/overview\nauth_errors:\n  - status: 401\n    type: AUTHORIZATION_ERROR\n    meaning: Missing Authorization header, or the token is invalid or expired.\n  - status: 402\n    type: WEBSITE_EXPIRED\n    meaning: The website that owns the token is in an expired billing state.\n  - status: 403\n    subtype: MISSING_SCOPE / OAUTH_TOKEN_REQUIRED / FORBIDDEN_RESOURCE\n    meaning: Token is valid but lacks\
  \ the permission, or the endpoint requires OAuth rather than an API key.\ngaps:\n  - oauth2 is documented but absent from the OpenAPI securitySchemes.\n  - No /.well-known/oauth-authorization-server or /.well-known/openid-configuration is served (404 on every host probed).\n  - API keys never expire and have no documented rotation path.\nevidence:\n  - url: https://developers.squarespace.com/commerce-apis/authentication-and-permissions\n    status: 200\n  - url: https://developers.squarespace.com/oauth\n    status: 200\n  - url: https://developers.squarespace.com/commerce-apis/making-requests\n    status: 200\n  - url: https://www.squarespace.com/.well-known/oauth-authorization-server\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/authentication/squarespace-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Commerce
- E-Commerce
- Marketing
- Payments
- Retail
- Website Builder
- Webhooks
---
