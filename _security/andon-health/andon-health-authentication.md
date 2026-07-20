---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Andon Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Andon Health secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Andon Health
provider_slug: andon-health
scheme_count: 2
schemes:
- description: iHealth Open API V2 authorizes third-party applications via OAuth 2.0. The developer portal issues client credentials and drives an authorization-code consent flow before an app may read a user's device data.
  docs: https://developer.ihealthlabs.com/
  endpoints:
    authorize: https://developer.ihealthlabs.com/api/public/oauth2/authorize
    consent: https://developer.ihealthlabs.com/api/public/oauth2/check-consent
    validate_client: https://developer.ihealthlabs.com/api/public/oauth2/validate-client
  evidence: developer.ihealthlabs.com JS bundle references /api/public/oauth2/* routes and OpenApiV2 application/user data paths; api.ihealthlabs.com returns HTTP 403 to unauthenticated requests.
  flow: authorizationCode
  name: ihealthOpenApiOAuth2
  resource_host: https://api.ihealthlabs.com
  type: oauth2
- authorization_endpoint: https://account.ihealthlabs.com/authentication/oauth/authorize
  description: The ihealthlabs.com storefront exposes the Shopify Customer Account API as an OpenID Connect provider (issuer shopify.com), used for shopper login, not for the health-device Open API.
  evidence: ihealthlabs.com/.well-known/openid-configuration (HTTP 200).
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg: RS256
  issuer: https://shopify.com/authentication/42894065826
  jwks_uri: https://account.ihealthlabs.com/authentication/.well-known/jwks.json
  name: shopifyCustomerAccount
  openid_configuration: well-known/andon-health-openid-configuration.json
  pkce: S256
  token_endpoint: https://account.ihealthlabs.com/authentication/oauth/token
  type: openIdConnect
slug: andon-health-authentication
source_filename: andon-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: >-\n  No first-party OpenAPI is published, so this profile is assembled from probed\n  live evidence: the iHealth Developer Portal SPA bundle\n  (developer.ihealthlabs.com) which references OAuth2 authorize/consent/validate\n  endpoints and OpenApiV2 application/user data resources on\n  api.ihealthlabs.com, plus the ihealthlabs.com storefront\n  /.well-known/openid-configuration (Shopify Customer Account API).\nsummary:\n  types:\n    - oauth2\n    - openIdConnect\nschemes:\n  - name: ihealthOpenApiOAuth2\n    type: oauth2\n    flow: authorizationCode\n    description: >-\n      iHealth Open API V2 authorizes third-party applications via OAuth 2.0.\n      The developer portal issues client credentials and drives an\n      authorization-code consent flow before an app may read a user's device\n      data.\n    endpoints:\n      authorize: https://developer.ihealthlabs.com/api/public/oauth2/authorize\n      consent: https://developer.ihealthlabs.com/api/public/oauth2/check-consent\n\
  \      validate_client: https://developer.ihealthlabs.com/api/public/oauth2/validate-client\n    resource_host: https://api.ihealthlabs.com\n    evidence: >-\n      developer.ihealthlabs.com JS bundle references /api/public/oauth2/*\n      routes and OpenApiV2 application/user data paths; api.ihealthlabs.com\n      returns HTTP 403 to unauthenticated requests.\n    docs: https://developer.ihealthlabs.com/\n  - name: shopifyCustomerAccount\n    type: openIdConnect\n    description: >-\n      The ihealthlabs.com storefront exposes the Shopify Customer Account API as\n      an OpenID Connect provider (issuer shopify.com), used for shopper login,\n      not for the health-device Open API.\n    openid_configuration: well-known/andon-health-openid-configuration.json\n    issuer: https://shopify.com/authentication/42894065826\n    token_endpoint: https://account.ihealthlabs.com/authentication/oauth/token\n    authorization_endpoint: https://account.ihealthlabs.com/authentication/oauth/authorize\n\
  \    jwks_uri: https://account.ihealthlabs.com/authentication/.well-known/jwks.json\n    id_token_signing_alg: RS256\n    pkce: S256\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n    evidence: ihealthlabs.com/.well-known/openid-configuration (HTTP 200).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andon-health/refs/heads/main/authentication/andon-health-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Healthcare
- Medical Devices
- Digital Health
- Remote Patient Monitoring
- Connected Health
- IoT
- Wearables
---
