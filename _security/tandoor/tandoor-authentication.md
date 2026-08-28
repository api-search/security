---
api_key_in: []
api_specs:
- filename: tandoor-api-openapi.yml
  format: yaml
  label: Tandoor API
  slug: tandoor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tandoor/refs/heads/main/openapi/tandoor-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Tandoor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tandoor Recipes declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Tandoor Recipes
provider_slug: tandoor
scheme_count: 3
schemes:
- detail: Declared globally via SPECTACULAR_SETTINGS.APPEND_COMPONENTS and applied to every operation via SPECTACULAR_SETTINGS.SECURITY. The contract does not state the token format or where to get one.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/tandoor-api-openapi.yml
  token_sources:
  - detail: Long-lived access tokens managed by the user in the application UI.
    operation: apiAccessTokenList / apiAccessTokenCreate (/api/access-token/)
  - detail: 'Exchanges {username, password} for a DRF auth token. Probed 2026-08-27 with an empty body: HTTP 400 {"username":["This field is required."],"password":["This field is required."]}. Subject to the login rate limiting added in 2.6.1.'
    operation: apiTokenAuthCreate (POST /api-token-auth/)
  type: apiKey
- declared_in_contract: false
  detail: rest_framework.authentication.SessionAuthentication is the first DEFAULT_AUTHENTICATION_CLASS. The Vue 3 frontend uses it. Requires CSRF handling and is not appropriate for an agent.
  in: cookie
  name: SessionAuth
  source: recipes/settings.py REST_FRAMEWORK.DEFAULT_AUTHENTICATION_CLASSES
  type: cookie
- declared_in_contract: false
  detail: 'django-oauth-toolkit is in INSTALLED_APPS and oauth2_provider.contrib.rest_framework. OAuth2Authentication is a DEFAULT_AUTHENTICATION_CLASS. settings.py defines OAUTH2_PROVIDER.SCOPES = {read, write, bookmarklet, mealplan}. But oauth2_provider.urls is not included in recipes/urls.py or cookbook/urls.py, so no endpoint is served: probes of https://app.tandoor.dev/o/authorize/ and https://app.tandoor.dev/o/token/ both returned 302 to /accounts/login/ (the Django catch-all) on 2026-08-27. No scopes/ artifact is written and no OAuthScopes pointer is emitted, because the scopes are not obtainable over HTTP.'
  name: OAuth2
  reachable: false
  scopes_in_code:
    bookmarklet: only access to bookmarklet
    mealplan: only access to mealplan
    read: Read scope
    write: Write scope
  type: oauth2
slug: tandoor-authentication
source_filename: tandoor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  openapi/tandoor-api-openapi.yml,\n  https://docs.tandoor.dev/features/authentication/,\n  https://github.com/TandoorRecipes/recipes/blob/develop/recipes/settings.py,\n  live probe of https://app.tandoor.dev/_allauth/app/v1/config and /api-token-auth/\ndocs: https://docs.tandoor.dev/features/authentication/\nsummary: >-\n  One scheme is declared in the contract — an access token in the `Authorization` header — and two\n  more work in practice: Django session cookies for browser clients, and the django-allauth headless\n  API for login flows. django-oauth-toolkit is installed and OAuth2Authentication is a default\n  authentication class with four scopes defined in settings, but the oauth2_provider URLs are not\n  routed, so there is no reachable authorize or token endpoint. Treat Tandoor as key-auth.\nsummary_structured:\n  types:\n    - apiKey\n  api_key_in:\n    - header\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n\
  \    in: header\n    parameter: Authorization\n    sources:\n      - openapi/tandoor-api-openapi.yml\n    detail: >-\n      Declared globally via SPECTACULAR_SETTINGS.APPEND_COMPONENTS and applied to every operation via\n      SPECTACULAR_SETTINGS.SECURITY. The contract does not state the token format or where to get one.\n    token_sources:\n      - operation: apiAccessTokenList / apiAccessTokenCreate (/api/access-token/)\n        detail: Long-lived access tokens managed by the user in the application UI.\n      - operation: apiTokenAuthCreate (POST /api-token-auth/)\n        detail: >-\n          Exchanges {username, password} for a DRF auth token. Probed 2026-08-27 with an empty body:\n          HTTP 400 {\"username\":[\"This field is required.\"],\"password\":[\"This field is required.\"]}.\n          Subject to the login rate limiting added in 2.6.1.\n  - name: SessionAuth\n    type: cookie\n    in: cookie\n    declared_in_contract: false\n    detail: >-\n      rest_framework.authentication.SessionAuthentication\
  \ is the first DEFAULT_AUTHENTICATION_CLASS.\n      The Vue 3 frontend uses it. Requires CSRF handling and is not appropriate for an agent.\n    source: recipes/settings.py REST_FRAMEWORK.DEFAULT_AUTHENTICATION_CLASSES\n  - name: OAuth2\n    type: oauth2\n    declared_in_contract: false\n    reachable: false\n    detail: >-\n      django-oauth-toolkit is in INSTALLED_APPS and oauth2_provider.contrib.rest_framework.\n      OAuth2Authentication is a DEFAULT_AUTHENTICATION_CLASS. settings.py defines\n      OAUTH2_PROVIDER.SCOPES = {read, write, bookmarklet, mealplan}. But oauth2_provider.urls is not\n      included in recipes/urls.py or cookbook/urls.py, so no endpoint is served: probes of\n      https://app.tandoor.dev/o/authorize/ and https://app.tandoor.dev/o/token/ both returned 302 to\n      /accounts/login/ (the Django catch-all) on 2026-08-27. No scopes/ artifact is written and no\n      OAuthScopes pointer is emitted, because the scopes are not obtainable over HTTP.\n    scopes_in_code:\n\
  \      read: Read scope\n      write: Write scope\n      bookmarklet: only access to bookmarklet\n      mealplan: only access to mealplan\ndefault_permission: rest_framework.permissions.IsAuthenticated\nunauthenticated_behaviour:\n  status: 302\n  detail: >-\n    An unauthenticated request to an /api/ path is REDIRECTED to /accounts/login/?next=<path> rather\n    than answered 401 or 403. Clients that follow redirects receive HTTP 200 and an HTML login form.\n    Disable redirect following. Observed 2026-08-27 on GET https://app.tandoor.dev/api/server-settings/.\n  exception: >-\n    GET /openapi/ is served WITHOUT authentication (HTTP 200, application/vnd.oai.openapi). It is the\n    only /-level API surface an anonymous caller can read.\nend_user_login:\n  framework: django-allauth (account, socialaccount, headless, mfa, usersessions)\n  headless_api:\n    base: /_allauth/\n    config: /_allauth/app/v1/config\n    probed: '2026-08-27'\n    status: 200\n    observed:\n      login_methods:\
  \ [username]\n      open_for_signup: true\n      mfa_supported: [recovery_codes, totp]\n      passkey_login: false\n      social_providers_on_hosted_instance: [facebook, google]\n  social_providers:\n    detail: >-\n      Operators enable providers with the SOCIAL_PROVIDERS environment variable and configure them\n      through SOCIALACCOUNT_PROVIDERS. Any allauth provider works, including a generic\n      openid_connect provider with PKCE against the operator's own IdP. This is INBOUND identity for\n      end users — it does not make Tandoor an OIDC provider and does not affect API authorization.\n    docs: https://docs.tandoor.dev/features/authentication/\nmtls: false\nopenid_connect_provider: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tandoor/refs/heads/main/authentication/tandoor-authentication.yml
summary_line: 3 schemes
tags:
- Recipes
- Meal Planning
- Food
- Nutrition
- Shopping Lists
- Open Source
- Self-Hosted
- Home Automation
- Django
- Open Data
---
