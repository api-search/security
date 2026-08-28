---
api_key_in: []
api_specs:
- filename: mealie-openapi.json
  format: json
  label: Mealie API
  slug: mealie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealie/refs/heads/main/openapi/mealie-openapi.json
auth_types:
- oauth2
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Mealie Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Mealie secures its APIs with oauth2 and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Mealie
provider_slug: mealie
scheme_count: 2
schemes:
- applied_to_operations: 230
  flows:
  - flow: password
    scopes: 0
    tokenUrl: /api/auth/token
  name: OAuth2PasswordBearer
  note: FastAPI's OAuth2 password flow. POST /api/auth/token with form-encoded username/password returns an access token; POST /api/auth/refresh refreshes it and POST /api/auth/logout ends the session.
  sources:
  - openapi/mealie-openapi.json
  type: oauth2
- docs: https://docs.mealie.io/documentation/getting-started/api-usage/
  expiry: long-lived (no stated expiry; revoked by deleting the token)
  format: Bearer <token>
  header: Authorization
  in: header
  minted_at: /user/profile/api-tokens
  name: API Token (bearer)
  note: Not declared as a separate securityScheme in the OpenAPI document — it is accepted by the same bearer handler as the password-flow token. This is the model the docs tell integrators to use.
  operations:
  - create_api_token_api_users_api_tokens_post
  - delete_api_token_api_users_api_tokens__token_id__delete
  scheme: bearer
  type: http
slug: mealie-authentication
source_filename: mealie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://docs.mealie.io/documentation/getting-started/api-usage/\ndocs: https://docs.mealie.io/documentation/getting-started/api-usage/\nspec_source: openapi/mealie-openapi.json\nsummary:\n  types:\n  - oauth2\n  - http-bearer\n  oauth2_flows:\n  - password\n  primary_model: long-lived bearer API token minted in the Mealie UI\n  note: >-\n    Mealie is self-hosted, so every instance is its own authorization server. The\n    OpenAPI document declares a single OAuth2 password-bearer scheme applied to 230\n    of 264 operations; in practice the documented way to call the API from a script\n    or a third-party integration is a long-lived API token created by the user at\n    /user/profile/api-tokens and sent as `Authorization: Bearer <token>`.\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /api/auth/token\n    scopes: 0\n  applied_to_operations: 230\n  sources:\n  - openapi/mealie-openapi.json\n\
  \  note: >-\n    FastAPI's OAuth2 password flow. POST /api/auth/token with form-encoded\n    username/password returns an access token; POST /api/auth/refresh refreshes it\n    and POST /api/auth/logout ends the session.\n- name: API Token (bearer)\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <token>'\n  minted_at: /user/profile/api-tokens\n  operations:\n  - create_api_token_api_users_api_tokens_post\n  - delete_api_token_api_users_api_tokens__token_id__delete\n  expiry: long-lived (no stated expiry; revoked by deleting the token)\n  docs: https://docs.mealie.io/documentation/getting-started/api-usage/\n  note: >-\n    Not declared as a separate securityScheme in the OpenAPI document — it is\n    accepted by the same bearer handler as the password-flow token. This is the\n    model the docs tell integrators to use.\nuser_login_methods:\n- method: local credentials\n  description: Username/password stored in the Mealie instance.\n- method: OpenID\
  \ Connect\n  description: >-\n    Mealie acts as an OIDC relying party against an external IdP (Authentik,\n    Authelia, Keycloak, Okta, Google, Entra ID). Requires the Authorization Code\n    flow with PKCE and a confidential client. Since v3.21.0 the IdP must assert\n    `email_verified` unless OIDC_REQUIRES_EMAIL_VERIFICATION=false.\n  docs: https://docs.mealie.io/documentation/getting-started/authentication/oidc-v2/\n  operations:\n  - oauth_login_api_auth_oauth_get\n  - oauth_callback_api_auth_oauth_callback_get\n  - oauth_native_config_api_auth_oauth_native_config_get\n  - oauth_native_token_api_auth_oauth_native_token_post\n- method: LDAP\n  description: Directory-backed login for self-hosted deployments.\n  docs: https://docs.mealie.io/documentation/getting-started/authentication/ldap/\nauthorization_model:\n  scheme: per-user permission flags plus group/household visibility\n  permissions:\n  - name: Administrator\n    allows: Access to administrator tools\n  - name: Invite\n\
  \    allows: Generating invitation links for other users\n  - name: Manage group\n    allows: Access to group management areas and settings\n  - name: Organize group data\n    allows: Creating, updating, deleting and merging foods, tags and categories\n  public_access: >-\n    Unauthenticated reads are possible through the /api/explore/groups/{group_slug}/*\n    surface only when the group is not private, the household is not private and\n    allows outside viewing, and the recipe itself is public. Private share links\n    bypass those checks.\n  docs: https://docs.mealie.io/documentation/getting-started/usage/permissions-and-public-access/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mealie/refs/heads/main/authentication/mealie-authentication.yml
summary_line: oauth2/http-bearer · 2 schemes
tags:
- Company
- Recipes
- Food
- Meal Planning
- Shopping Lists
- Self-Hosted
- Open Source
- Household
- Nutrition
- Home Automation
---
