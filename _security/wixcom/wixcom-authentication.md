---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: Wix authentication profile captured from the developer docs (Wix publishes no OpenAPI, so this is docs-searched rather than spec-derived). Every Wix API call is authenticated as one of four identities (Wix user, app, site member, site visitor). Admin/server calls use an API key from the API Keys Manager in the Authorization header plus a wix-account-id (account-level) or wix-site-id (site-level) header. Wix apps use OAuth 2 client credentials (Create Access Token with app ID, app secret, and app instance ID) yielding Bearer access tokens; the redirect-based "custom authentication" flow is legacy and closed to new apps. Headless/site-member auth uses OAuthStrategy with a client ID for member and visitor tokens. Elevated permissions let backend code raise an identity's permissions for specific calls.
kind: authentication
layout: security
method: searched
name: Wixcom Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Wix.com secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Wix.com
provider_slug: wixcom
scheme_count: 3
schemes:
- additional_headers:
  - name: wix-account-id
    usage: required for account-level API calls
  - name: wix-site-id
    usage: required for site-level API calls (one of the two, never both)
  docs: https://dev.wix.com/docs/api-reference/articles/authentication/api-keys/about-api-keys
  in: header
  key_manager: https://manage.wix.com/account/api-keys
  name: ApiKey
  parameter: Authorization
  type: apiKey
- docs: https://dev.wix.com/docs/build-apps/develop-your-app/access/authentication/about-oauth
  flow: clientCredentials
  name: OAuth2ClientCredentials
  notes: Legacy "custom authentication" (authorization-code style with a 10-minute authorization code and non-expiring refresh tokens) is deprecated and unavailable to new apps.
  token_operation: Create Access Token (https://dev.wix.com/docs/api-reference/app-management/oauth-2/create-access-token) called with app ID, app secret, and app instance ID.
  token_type: Bearer
  type: oauth2
- audience: headless clients, site members and visitors
  docs: https://dev.wix.com/docs/go-headless/self-managed-headless/authentication
  name: OAuthStrategy
  notes: '@wix/sdk OAuthStrategy with an OAuth-app client ID issues visitor and member tokens for headless projects.'
  type: oauth2
slug: wixcom-authentication
source_filename: wixcom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://dev.wix.com/docs/api-reference/articles/authentication\nsource: >-\n  https://dev.wix.com/docs/api-reference/articles/authentication/api-keys/make-api-calls-with-an-api-key\n  + https://dev.wix.com/docs/build-apps/develop-your-app/access/authentication/about-oauth\n  + https://dev.wix.com/docs/api-reference/app-management/oauth-2/introduction\ndescription: >-\n  Wix authentication profile captured from the developer docs (Wix publishes\n  no OpenAPI, so this is docs-searched rather than spec-derived). Every Wix\n  API call is authenticated as one of four identities (Wix user, app, site\n  member, site visitor). Admin/server calls use an API key from the API Keys\n  Manager in the Authorization header plus a wix-account-id (account-level)\n  or wix-site-id (site-level) header. Wix apps use OAuth 2 client credentials\n  (Create Access Token with app ID, app secret, and app instance ID) yielding\n  Bearer access tokens;\
  \ the redirect-based \"custom authentication\" flow is\n  legacy and closed to new apps. Headless/site-member auth uses OAuthStrategy\n  with a client ID for member and visitor tokens. Elevated permissions let\n  backend code raise an identity's permissions for specific calls.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  identities: [WIX_USER, APP, MEMBER, ANONYMOUS_VISITOR]\nschemes:\n  - name: ApiKey\n    type: apiKey\n    in: header\n    parameter: Authorization\n    additional_headers:\n      - name: wix-account-id\n        usage: required for account-level API calls\n      - name: wix-site-id\n        usage: required for site-level API calls (one of the two, never both)\n    key_manager: https://manage.wix.com/account/api-keys\n    docs: https://dev.wix.com/docs/api-reference/articles/authentication/api-keys/about-api-keys\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_operation:\
  \ >-\n      Create Access Token\n      (https://dev.wix.com/docs/api-reference/app-management/oauth-2/create-access-token)\n      called with app ID, app secret, and app instance ID.\n    token_type: Bearer\n    docs: https://dev.wix.com/docs/build-apps/develop-your-app/access/authentication/about-oauth\n    notes: >-\n      Legacy \"custom authentication\" (authorization-code style with a\n      10-minute authorization code and non-expiring refresh tokens) is\n      deprecated and unavailable to new apps.\n  - name: OAuthStrategy\n    type: oauth2\n    audience: headless clients, site members and visitors\n    docs: https://dev.wix.com/docs/go-headless/self-managed-headless/authentication\n    notes: >-\n      @wix/sdk OAuthStrategy with an OAuth-app client ID issues visitor and\n      member tokens for headless projects.\nelevated_permissions:\n  docs: https://dev.wix.com/docs/api-reference/articles/authentication/about-elevated-permissions\nsdk_strategies: [ApiKeyStrategy, OAuthStrategy]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wixcom/refs/heads/main/authentication/wixcom-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Website Builder
- eCommerce
- CMS
- Bookings
- Payments
- Headless
- SaaS
- No Code
---
