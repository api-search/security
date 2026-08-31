---
api_key_in: []
api_specs:
- filename: strivacity-admin-portal-openapi.yml
  format: yaml
  label: Strivacity Admin API
  slug: strivacity-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strivacity/refs/heads/main/openapi/strivacity-admin-portal-openapi.yml
- filename: strivacity-myaccount-portal-openapi.yml
  format: yaml
  label: Strivacity MyAccount API
  slug: strivacity-myaccount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strivacity/refs/heads/main/openapi/strivacity-myaccount-portal-openapi.yml
- filename: strivacity-native-journey-openapi.yml
  format: yaml
  label: Strivacity Journey Flow API
  slug: strivacity-journey-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strivacity/refs/heads/main/openapi/strivacity-native-journey-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Strivacity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Strivacity secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Strivacity
provider_slug: strivacity
scheme_count: 2
schemes:
- applies_to:
  - openapi/strivacity-admin-portal-openapi.yml
  - openapi/strivacity-admin-management-openapi.yml
  - openapi/strivacity-myaccount-portal-openapi.yml
  - openapi/strivacity-native-journey-openapi.yml
  header: 'Authorization: Bearer <access_token>'
  name: securityScheme
  scheme: bearer
  type: http
- applies_to:
  - openapi/strivacity-admin-console-getting-started-openapi.yml
  name: basicAuth
  note: HTTP Basic here is the client-credentials presentation at the token endpoint — client_id as username, client_secret as password — not a Basic-auth data API.
  scheme: basic
  type: http
slug: strivacity-authentication
source_filename: strivacity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://docs.strivacity.com/reference/getting-started-with-the-admin-api ,\n  https://docs.strivacity.com/docs/rest-api-access-policies ,\n  https://docs.strivacity.com/docs/api-sec-policy ,\n  plus derived from openapi/_original/*.json securitySchemes\ndocs: https://docs.strivacity.com/reference/getting-started-with-the-admin-api\nsummary:\n  types:\n  - http\n  - oauth2\n  primary: OAuth 2.0 client credentials -> opaque or JWT bearer access token\nmodel: >-\n  Every Strivacity REST API is bearer-token protected. Tokens are minted by the tenant's own OAuth 2.0\n  token endpoint using the client-credentials grant, with BOTH a scope set and an audience. Authorization\n  is two-sided: the token must carry the scope, and an API Access policy inside the instance must have\n  granted that scope to that client. Requesting a scope the policy does not grant fails — possession of\n  valid client credentials is not by itself access.\n\
  schemes:\n- name: securityScheme\n  type: http\n  scheme: bearer\n  applies_to:\n  - openapi/strivacity-admin-portal-openapi.yml\n  - openapi/strivacity-admin-management-openapi.yml\n  - openapi/strivacity-myaccount-portal-openapi.yml\n  - openapi/strivacity-native-journey-openapi.yml\n  header: 'Authorization: Bearer <access_token>'\n- name: basicAuth\n  type: http\n  scheme: basic\n  applies_to:\n  - openapi/strivacity-admin-console-getting-started-openapi.yml\n  note: >-\n    HTTP Basic here is the client-credentials presentation at the token endpoint — client_id as username,\n    client_secret as password — not a Basic-auth data API.\noauth2:\n  declared_in_spec: false\n  spec_gap: >-\n    The published OpenAPI documents describe the bearer token but never declare an oauth2 securityScheme\n    with its token URL and scopes, so a generated client cannot obtain a token from the spec alone. The\n    flow is fully documented in prose instead. This is the single largest machine-readability\
  \ gap in an\n    otherwise complete contract set.\n  grant_types:\n  - client_credentials\n  - authorization_code\n  token_endpoint: https://{tenant}.strivacity.com/oauth2/token\n  token_endpoint_auth: client_secret_basic (client_id as username, client_secret as password)\n  audience_parameter: required\n  resource_parameter:\n    supported: true\n    rfc: RFC 8707\n    note: >-\n      Agents and OAuth clients name the target protected resource (an MCP server or API registered in\n      Strivacity) in the `resource` parameter on both the authorization and token request. Strivacity\n      matches it exactly against the resources assigned to the client and makes it the token audience.\n  pkce: required for authorization-code flows\n  token_format: opaque by default; JWT selectable per client so resource servers can validate locally\n  token_lifetime_example: 3599 seconds\n  scopes_artifact: scopes/strivacity-scopes.yml\n  scope_count: 106\noidc:\n  discovery: https://{tenant}.strivacity.com/.well-known/openid-configuration\n\
  \  rfc8414_oauth_authorization_server: false\n  rfc8414_note: >-\n    Strivacity states explicitly that the RFC 8414 /.well-known/oauth-authorization-server path is not\n    published, and that conforming MCP clients are expected to fall back to OIDC Discovery.\n  jwks: published in the OIDC discovery metadata\n  client_id_metadata_document: >-\n    When enabled, discovery advertises client_id_metadata_document_supported: true, letting external AI\n    agents self-identify as dynamic clients without pre-registration.\nend_user_authentication:\n  note: >-\n    Distinct from API authentication. Strivacity is itself the customer-facing authentication product —\n    passwords, magic links, SMS/email/voice passcodes, soft tokens, FIDO2 / WebAuthn passkeys, platform\n    biometrics, social and enterprise federation (OIDC + SAML2), plus adaptive step-up driven by risk\n    policy.\n  standards:\n  - OpenID Connect\n  - OAuth 2.0 / 2.1\n  - SAML 2.0\n  - FIDO2 / WebAuthn\n  - RFC 9700 OAuth 2.0\
  \ Security Best Current Practice\n  - RFC 8707 Resource Indicators\n  - Token Exchange\n  - CIBA\n  - DPoP\n  - PAR\n  - RAR\npolicy_layer:\n  name: API Access policy (API security policy)\n  docs: https://docs.strivacity.com/docs/api-sec-policy\n  note: >-\n    Scopes are attached to clients through an API Access policy assignment. Only clients created as\n    \"OIDC using no-code components\" can be assigned one; other client types will not appear in the\n    assignment dropdown.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strivacity/refs/heads/main/authentication/strivacity-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Identity
- customer-identity-and-access-management
- ciam
- Authentication
- Authorization
- openid-connect
- consent-management
- multi-factor-authentication
- Identity Verification
- fraud-detection
- agentic-identity
- Security
---
