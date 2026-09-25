---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Aible protects its API with opaque bearer session tokens, not API keys and not a public OAuth 2.0 authorization server. The published route index states it plainly: "Nearly all API operations are protected and require a header (Authorization) set to a string beginning with Bearer ... where ... is your authenticated session token." Three token classes exist — user token, tenant token, and a short-lived STS token scoped to a route set — and the route index labels every route with the class it requires. Enterprise SSO (SAML 2.0, OAuth 2.0 authorization-code reply, Microsoft Entra/Azure, and Google Cloud IAP) is supported for interactive sign-in. No OpenAPI securitySchemes block exists because Aible publishes no OpenAPI; everything below is read from the provider''s own route index and from live unauthenticated probes of the API host.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aible Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aible declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Aible
provider_slug: aible
scheme_count: 1
schemes:
- applies_to: nearly all /v1 routes
  description: Opaque session token issued by the login routes. Expires; renewable before expiry via the renewal routes below rather than by re-authenticating.
  format: Bearer <session token>
  id: bearer-session-token
  in: header
  parameter: Authorization
  scheme: bearer
  type: http
slug: aible-authentication
source_filename: aible-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://api.iamaible.com/\nname: Aible API authentication\ndescription: >-\n  Aible protects its API with opaque bearer session tokens, not API keys and not a public\n  OAuth 2.0 authorization server. The published route index states it plainly: \"Nearly all\n  API operations are protected and require a header (Authorization) set to a string beginning\n  with Bearer ... where ... is your authenticated session token.\" Three token classes exist —\n  user token, tenant token, and a short-lived STS token scoped to a route set — and the route\n  index labels every route with the class it requires. Enterprise SSO (SAML 2.0, OAuth 2.0\n  authorization-code reply, Microsoft Entra/Azure, and Google Cloud IAP) is supported for\n  interactive sign-in. No OpenAPI securitySchemes block exists because Aible publishes no\n  OpenAPI; everything below is read from the provider's own route index and from live\n  unauthenticated probes of the\
  \ API host.\ndocs: https://api.iamaible.com/\nx-evidence:\n  fetched: '2026-09-14'\n  route_index:\n    url: https://api.iamaible.com/\n    http_status: 200\n  unauthenticated_probe:\n    url: https://api.iamaible.com/v1/me\n    http_status: 403\n    body: '{\"type\":\"Invalid Token\",\"message\":\"Unable to locate Authorization header!\",\"key\":null}'\n    note: >-\n      Aible answers a missing Authorization header with 403, not 401, and returns no\n      WWW-Authenticate challenge header.\n\nsummary:\n  auth_types:\n  - http-bearer\n  api_key_locations: []\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  public_authorization_server: false\n  sso_federation:\n  - saml2\n  - oauth2-authorization-code\n  - microsoft-entra\n  - google-cloud-iap\n  token_classes: 3\n  routes_requiring_tenant_token: 349\n  routes_requiring_user_token: 9\n  routes_requiring_any_token: 10\n  routes_unlabelled: 26\n\nschemes:\n- id: bearer-session-token\n  type: http\n  scheme: bearer\n\
  \  in: header\n  parameter: Authorization\n  format: 'Bearer <session token>'\n  description: >-\n    Opaque session token issued by the login routes. Expires; renewable before expiry via the\n    renewal routes below rather than by re-authenticating.\n  applies_to: nearly all /v1 routes\n\ntoken_classes:\n- id: user-token\n  label: user token\n  description: Identifies a human user session. Used by /v1/me, /v1/logout and the user-token renewal route.\n  renew:\n    operation: login.renew_user_token\n    method: POST\n    path: /v1/renew/login\n  routes_labelled: 9\n- id: tenant-token\n  label: tenant token\n  description: >-\n    Identifies a tenant (workspace/organization) context. This is the dominant token class —\n    349 of 394 published routes are labelled \"requires tenant token\".\n  renew:\n    operation: tenant.renew_token\n    method: POST\n    path: /v1/renew/tenant\n  routes_labelled: 349\n- id: sts-token\n  label: short-lived STS token\n  description: >-\n    \"Allocate\
  \ a short lived session token restricted to routes.\" Minted from a tenant token and\n    scoped down to a named route set — the closest thing Aible publishes to a scope model.\n  mint:\n    operation: tenant.create_sts_token\n    method: POST\n    path: /v1/tenant/<tenant_id:int>/sts\n  related:\n    - operation: account.create_foreign_sts_token\n      method: POST\n      path: /v1/account/<id:int>/foreign_sts\n      note: >-\n        Mints credentials for the customer's own cloud account so a client can call the Cloud\n        Account API directly, or relay through /v1/account/<id>/communicate.\n  routes_labelled: 0\n  note: >-\n    STS tokens are not a separate label in the route index; they are accepted in place of a\n    tenant token on relay routes, per the account.communicate docstring.\n\nflows:\n- id: password-login\n  description: Email + password sign-in returning a user session.\n  steps:\n  - operation: login.login_user\n    method: POST\n    path: /v1/login\n    body: '{\"\
  email\": str}'\n    note: Returns a ProvisionalLoginRequest — the tenant/SSO discovery step.\n  - operation: login.check_password\n    method: POST\n    path: /v1/login/password\n    body: '{\"token\": str, \"password\": str}'\n    note: Returns a UserSession carrying the bearer token.\n- id: saml-sso\n  description: SAML 2.0 service-provider-initiated SSO, per tenant.\n  steps:\n  - operation: login.service_provider_initiated_login\n    method: POST\n    path: /v1/login/by/<tenant_id:int>/via/<key:str>\n  - operation: login.saml_reply\n    method: POST\n    path: /v1/login/saml-reply\n    note: SAML ACS endpoint.\n  - operation: login.service_provider_initiated_logout_reply\n    method: POST\n    path: /v1/logout/saml-reply\n- id: oauth2-sso\n  description: >-\n    OAuth 2.0 authorization-code reply handler. Aible acts as the OAuth CLIENT here; it does not\n    publish an authorization server of its own, and no /.well-known/oauth-authorization-server or\n    /.well-known/openid-configuration\
  \ document is served on any Aible host.\n  steps:\n  - operation: login.oauth2_reply\n    method: GET\n    path: /v1/login/oauth2-reply\n    body: '{\"code\": str, \"state\": str}'\n- id: microsoft-entra-sso\n  description: Microsoft Entra ID / Azure AD authorization reply.\n  steps:\n  - operation: login.on_azure_authorized_get\n    method: GET\n    path: /v1/login/azure/authorized\n  - operation: login.on_azure_authorized_post\n    method: POST\n    path: /v1/login/azure/authorized\n- id: google-cloud-iap\n  description: Identity-Aware Proxy initiated sign-in, for Aible deployments fronted by Google Cloud IAP.\n  steps:\n  - operation: login.iap_initiated\n    method: GET\n    path: /v1/login/iap\n- id: lookup-token\n  description: >-\n    \"Generates a random lookup token and associates it with the tenant's API token.\" A tenant-scoped\n    indirection so a third party can validate a handed-out token without holding the tenant token.\n  steps:\n  - operation: login.create_lookup_token\n\
  \    method: POST\n    path: /v1/lookup-token\n  - operation: login.validate_lookup_token\n    method: POST\n    path: /v1/lookup-token/validate\n\nfederation:\n- id: tenant-foreign-authentication\n  description: >-\n    Per-tenant identity-provider registrations, managed over the API rather than only in a console.\n  operations:\n  - {method: GET,    path: /v1/foreign-authentications, id: tenant.list_foreign_authentications}\n  - {method: POST,   path: /v1/foreign-authentications, id: tenant.create_foreign_authentication}\n  - {method: GET,    path: /v1/foreign-authentication/<key_or_id:str>, id: tenant.get_foreign_authentication}\n  - {method: PATCH,  path: /v1/foreign-authentication/<key_or_id:str>, id: tenant.update_foreign_authentication}\n  - {method: DELETE, path: /v1/foreign-authentication/<key_or_id:str>, id: tenant.delete_foreign_authentication}\n\ngaps:\n- No machine-readable securityScheme declaration (no OpenAPI, Swagger or AsyncAPI is published).\n- No OAuth 2.0 scope model;\
  \ the nearest equivalent is the route-restricted STS token.\n- No /.well-known/oauth-authorization-server, /.well-known/openid-configuration or\n  /.well-known/oauth-protected-resource on any Aible host (all 404 on api.iamaible.com and\n  aible.com; iamaible.com answers 200 with an SPA shell, which is not a document).\n- Missing credentials return 403 without a WWW-Authenticate header, so a client cannot discover\n  the scheme from the challenge.\n- No public authentication guide outside the route index; the support community at\n  aible.zendesk.com is closed to the public (403).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aible/refs/heads/main/authentication/aible-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Machine Learning
- AutoML
- Analytics
- Data Science
- AI Agents
- Generative AI
- Enterprise Software
- Cloud
- Company
---
