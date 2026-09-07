---
anonymous_access: true
api_key_in: []
auth_types: []
description: Acadio publishes no OpenAPI and therefore no securitySchemes block. Its authentication surface is documented in the knowledge base as three distinct mechanisms — inbound JWT single sign-on into the LMS, Google OAuth 2.0 as a login provider, and HMAC request signing on the outbound webhook bus — plus a Shopify-supplied OpenID Connect provider on the storefront domain.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Acadio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acadio declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Acadio
provider_slug: acadio
scheme_count: 5
schemes:
- bearer_format: JWT
  credential: shared secret (symmetric), configured per tenant
  direction: inbound
  endpoint: https://{domain}/auth/callback/jwt-auth?token={token}&go={path}
  endpoint_note: '{domain} is the tenant''s Acadio domain or custom domain. The optional go parameter controls the post-authentication landing path; omitted, the user lands on the dashboard.'
  id: jwt-auth
  optional_claims:
  - max-age
  - issuer
  payload_fields:
  - description: The user's unique email address.
    name: email
    required: true
    type: string
  - name: firstName
    required: false
    type: string
  - name: lastName
    required: false
    type: string
  - description: Custom JSON data to associate with the user.
    name: meta
    required: false
    type: object
  - description: A list of group IDs to associate with the user. Full synchronization semantics.
    name: groups
    required: false
    type: array
  - description: A list of Credit objects (orderId string max 32 chars, id integer) to associate with the user.
    name: credits
    required: false
    type: array
  - description: When true, a newly created user is redirected to onboarding.
    name: onboard
    required: false
    type: boolean
  purpose: Create and/or authenticate users from the customer's own systems (single sign-on). The customer signs a JWT server-side with a shared secret configured in the Acadio Admin portal under Settings > Integrations > JWT Auth.
  scheme: bearer
  security_guidance: Acadio states the signing secret must be kept strictly server-side, that token generation must happen only in a trusted server environment, and that tokens should be short-lived via the max-age claim. Removing the integration causes Acadio to reject the secret and all signed tokens.
  surface: Acadio LMS (student and admin portals)
  type: http
- credential: Tenant-supplied Google Cloud OAuth 2.0 Client ID and Client Secret, entered in the Acadio Admin portal under Settings > Apps > Google OAuth 2.0.
  direction: inbound
  flow: authorization_code
  id: google-oauth2
  javascript_origins:
  - https://{your domain}.acadio.com
  - https://admin.acadio.com
  note: The Google OAuth 2.0 app is only available to authenticated registered users.
  purpose: Single sign-on with Google as the identity provider.
  redirect_uris:
  - https://{your domain}.acadio.com/auth/callback/google-oauth
  - https://admin.acadio.com/auth/callback/google-oauth
  surface: Acadio LMS (student and admin portals)
  type: oauth2
- algorithm: HMAC SHA-256
  credential: per-integration secret key created by the tenant
  direction: outbound
  header: X-Acadio-Hmac-Sha256
  id: webhook-hmac
  purpose: Lets a subscriber verify a delivered payload originated from Acadio and was not altered.
  surface: Acadio LMS webhook deliveries
  type: signature
- authorization_endpoint: https://shopify.com/authentication/78091452669/oauth/authorize
  direction: inbound
  discovery: https://acadio.com/.well-known/openid-configuration
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-accounts-oidc
  id_token_signing_alg: RS256
  issuer: https://shopify.com/authentication/78091452669
  jwks_uri: https://shopify.com/authentication/78091452669/.well-known/jwks.json
  note: Provided by the Shopify customer-accounts platform and served from Acadio's own domain. The issuer is a Shopify authentication tenant scoped to Acadio's shop (78091452669), so the document is Acadio's storefront identity surface rather than a generic Shopify one.
  pkce: S256
  surface: acadio.com storefront (course purchases)
  token_endpoint: https://shopify.com/authentication/78091452669/oauth/token
  type: openIdConnect
- direction: inbound
  id: ucp-mcp-anonymous
  purpose: The Universal Commerce Protocol MCP endpoint answers tools/list with no credential. Payment on complete_checkout is authorized by the buyer through a payment handler (Google Pay or Shopify card), not by an API credential.
  surface: https://acadio.com/api/ucp/mcp
  type: none
  verified: probed 2026-09-06 (HTTP 200, unauthenticated)
slug: acadio-authentication
source_filename: acadio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://acadio.instantdocsbase.com/help/jwt-auth-documentation ,\n  https://acadio.instantdocsbase.com/help/google-oauth-2-dot-0-documentation ,\n  https://acadio.instantdocsbase.com/help/webhooks-documentation , and the probed\n  https://acadio.com/.well-known/openid-configuration\ndocs: https://acadio.instantdocsbase.com/help/jwt-auth-documentation\ndescription: >-\n  Acadio publishes no OpenAPI and therefore no securitySchemes block. Its authentication surface is\n  documented in the knowledge base as three distinct mechanisms — inbound JWT single sign-on into\n  the LMS, Google OAuth 2.0 as a login provider, and HMAC request signing on the outbound webhook\n  bus — plus a Shopify-supplied OpenID Connect provider on the storefront domain.\nschemes:\n- id: jwt-auth\n  surface: Acadio LMS (student and admin portals)\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  direction: inbound\n  purpose: >-\n    Create\
  \ and/or authenticate users from the customer's own systems (single sign-on). The customer\n    signs a JWT server-side with a shared secret configured in the Acadio Admin portal under\n    Settings > Integrations > JWT Auth.\n  endpoint: https://{domain}/auth/callback/jwt-auth?token={token}&go={path}\n  endpoint_note: >-\n    {domain} is the tenant's Acadio domain or custom domain. The optional go parameter controls the\n    post-authentication landing path; omitted, the user lands on the dashboard.\n  credential: shared secret (symmetric), configured per tenant\n  optional_claims:\n  - max-age\n  - issuer\n  payload_fields:\n  - name: email\n    required: true\n    type: string\n    description: The user's unique email address.\n  - name: firstName\n    required: false\n    type: string\n  - name: lastName\n    required: false\n    type: string\n  - name: meta\n    required: false\n    type: object\n    description: Custom JSON data to associate with the user.\n  - name: groups\n   \
  \ required: false\n    type: array\n    description: A list of group IDs to associate with the user. Full synchronization semantics.\n  - name: credits\n    required: false\n    type: array\n    description: A list of Credit objects (orderId string max 32 chars, id integer) to associate with the user.\n  - name: onboard\n    required: false\n    type: boolean\n    description: When true, a newly created user is redirected to onboarding.\n  security_guidance: >-\n    Acadio states the signing secret must be kept strictly server-side, that token generation must\n    happen only in a trusted server environment, and that tokens should be short-lived via the\n    max-age claim. Removing the integration causes Acadio to reject the secret and all signed tokens.\n- id: google-oauth2\n  surface: Acadio LMS (student and admin portals)\n  type: oauth2\n  flow: authorization_code\n  direction: inbound\n  purpose: Single sign-on with Google as the identity provider.\n  redirect_uris:\n  - https://{your\
  \ domain}.acadio.com/auth/callback/google-oauth\n  - https://admin.acadio.com/auth/callback/google-oauth\n  javascript_origins:\n  - https://{your domain}.acadio.com\n  - https://admin.acadio.com\n  credential: >-\n    Tenant-supplied Google Cloud OAuth 2.0 Client ID and Client Secret, entered in the Acadio Admin\n    portal under Settings > Apps > Google OAuth 2.0.\n  note: The Google OAuth 2.0 app is only available to authenticated registered users.\n- id: webhook-hmac\n  surface: Acadio LMS webhook deliveries\n  type: signature\n  algorithm: HMAC SHA-256\n  direction: outbound\n  header: X-Acadio-Hmac-Sha256\n  credential: per-integration secret key created by the tenant\n  purpose: Lets a subscriber verify a delivered payload originated from Acadio and was not altered.\n- id: shopify-customer-accounts-oidc\n  surface: acadio.com storefront (course purchases)\n  type: openIdConnect\n  direction: inbound\n  discovery: https://acadio.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/78091452669\n\
  \  authorization_endpoint: https://shopify.com/authentication/78091452669/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/78091452669/oauth/token\n  jwks_uri: https://shopify.com/authentication/78091452669/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  pkce: S256\n  id_token_signing_alg: RS256\n  note: >-\n    Provided by the Shopify customer-accounts platform and served from Acadio's own domain. The\n    issuer is a Shopify authentication tenant scoped to Acadio's shop (78091452669), so the document\n    is Acadio's storefront identity surface rather than a generic Shopify one.\n- id: ucp-mcp-anonymous\n  surface: https://acadio.com/api/ucp/mcp\n  type: none\n  direction: inbound\n  purpose: >-\n    The Universal Commerce Protocol MCP endpoint answers tools/list with no credential. Payment on\n    complete_checkout is authorized by the buyer through a payment handler (Google Pay\
  \ or Shopify\n    card), not by an API credential.\n  verified: probed 2026-09-06 (HTTP 200, unauthenticated)\ngaps:\n- >-\n  No API key, no bearer-token API credential and no documented machine-to-machine authentication for\n  the api.acadio.com gateway. Every documented mechanism authenticates a HUMAN into the LMS or signs\n  an outbound event; none of them lets a third-party program call an Acadio LMS resource.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acadio/refs/heads/main/authentication/acadio-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Education
- Learning Management System
- Professional Education
- Continuing Education
- Certification
- Exam Preparation
- SCORM
- Webhooks
- Agentic Commerce
---
