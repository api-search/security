---
anonymous_access: false
api_key_in: []
auth_types:
- openIdConnect
- oauth2
- saml2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Cvent Community Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Cvent Community secures its APIs with openIdConnect, oauth2, and saml2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Cvent Community
provider_slug: cvent-community
scheme_count: 2
schemes:
- authorization_endpoint: https://support.cvent.com/services/oauth2/authorize
  code_challenge_methods_supported:
  - S256
  dpop_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  - EdDSA
  dynamic_client_registration: true
  end_session_endpoint: https://support.cvent.com/services/auth/idp/oidc/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://support.cvent.com/services/oauth2/introspect
  issuer: https://support.cvent.com
  jwks_uri: https://support.cvent.com/id/keys
  name: support-cvent-oidc
  openIdConnectUrl: https://support.cvent.com/.well-known/openid-configuration
  pkce: true
  platform: Salesforce Experience Cloud
  provenance_note: The endpoint set, claims list and scope list are Salesforce Experience Cloud's standard shape, served under Cvent's own domain by Cvent's Salesforce org. The issuer is https://support.cvent.com, so the document is Cvent's; the vocabulary inside it is the vendor's. Do not read the scope list as a Cvent-authored permission taxonomy.
  registration_endpoint: https://support.cvent.com/services/oauth2/register
  revocation_endpoint: https://support.cvent.com/services/oauth2/revoke
  scopes: scopes/cvent-community-scopes.yml
  sources:
  - well-known/cvent-community-openid-configuration.json
  surface: https://support.cvent.com/ (Knowledge Base, case management, Passkey support)
  token_endpoint: https://support.cvent.com/services/oauth2/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
  userinfo_endpoint: https://support.cvent.com/services/oauth2/userinfo
- binding: HttpRedirect
  interactive_login: https://community.cvent.com/login
  login_endpoint: https://community.cvent.com/HigherLogic/Security/SAML/localSAMLLoginService.aspx
  name: community-cvent-saml-sso
  note: The community front door is a Higher Logic SAML service provider that redirects to Cvent's IdP. No SAML metadata document is published at a discoverable path; the binding is read from the login link in the served page markup.
  platform: Higher Logic Thrive
  sources:
  - https://community.cvent.com/home
  surface: https://community.cvent.com/ (Cvent Community — forums, education, learning centers)
  type: saml2
slug: cvent-community-authentication
source_filename: cvent-community-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  https://support.cvent.com/.well-known/openid-configuration (HTTP 200, application/json, fetched\n  2026-09-07, saved verbatim to well-known/cvent-community-openid-configuration.json);\n  https://community.cvent.com/HigherLogic/Security/SAML/localSAMLLoginService.aspx (SAML login link\n  present in the community page markup, observed 2026-09-07)\ndocs: https://support.cvent.com/s/knowledgebase\nsummary:\n  types:\n    - openIdConnect\n    - oauth2\n    - saml2\n  api_key_in: []\n  oauth2_flows:\n    - authorizationCode\n    - refreshToken\n  note: >-\n    Cvent Community publishes no API contract, so this is an identity/SSO profile rather than an API\n    authentication profile. Two sign-in surfaces are observable without credentials.\nschemes:\n  - name: support-cvent-oidc\n    type: openIdConnect\n    surface: https://support.cvent.com/ (Knowledge Base, case management, Passkey support)\n    platform: Salesforce Experience\
  \ Cloud\n    openIdConnectUrl: https://support.cvent.com/.well-known/openid-configuration\n    issuer: https://support.cvent.com\n    authorization_endpoint: https://support.cvent.com/services/oauth2/authorize\n    token_endpoint: https://support.cvent.com/services/oauth2/token\n    userinfo_endpoint: https://support.cvent.com/services/oauth2/userinfo\n    revocation_endpoint: https://support.cvent.com/services/oauth2/revoke\n    introspection_endpoint: https://support.cvent.com/services/oauth2/introspect\n    registration_endpoint: https://support.cvent.com/services/oauth2/register\n    end_session_endpoint: https://support.cvent.com/services/auth/idp/oidc/logout\n    jwks_uri: https://support.cvent.com/id/keys\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n    token_endpoint_auth_methods_supported:\n      - client_secret_post\n      - client_secret_basic\n      - private_key_jwt\n    code_challenge_methods_supported:\n      - S256\n    id_token_signing_alg_values_supported:\n\
  \      - RS256\n    dpop_signing_alg_values_supported:\n      - RS256\n      - RS384\n      - RS512\n      - ES256\n      - ES384\n      - ES512\n      - EdDSA\n    dynamic_client_registration: true\n    pkce: true\n    scopes: scopes/cvent-community-scopes.yml\n    sources:\n      - well-known/cvent-community-openid-configuration.json\n    provenance_note: >-\n      The endpoint set, claims list and scope list are Salesforce Experience Cloud's standard shape,\n      served under Cvent's own domain by Cvent's Salesforce org. The issuer is https://support.cvent.com,\n      so the document is Cvent's; the vocabulary inside it is the vendor's. Do not read the scope list\n      as a Cvent-authored permission taxonomy.\n  - name: community-cvent-saml-sso\n    type: saml2\n    surface: https://community.cvent.com/ (Cvent Community — forums, education, learning centers)\n    platform: Higher Logic Thrive\n    login_endpoint: https://community.cvent.com/HigherLogic/Security/SAML/localSAMLLoginService.aspx\n\
  \    binding: HttpRedirect\n    interactive_login: https://community.cvent.com/login\n    note: >-\n      The community front door is a Higher Logic SAML service provider that redirects to Cvent's IdP.\n      No SAML metadata document is published at a discoverable path; the binding is read from the\n      login link in the served page markup.\n    sources:\n      - https://community.cvent.com/home\nmcp_authorization:\n  status: not-enabled\n  note: >-\n    community.cvent.com answers both RFC 8414 and RFC 9728 discovery paths with a JSON error stating\n    the Higher Logic MCP server is not enabled for tenant CVENT. See mcp/cvent-community-mcp.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-community/refs/heads/main/authentication/cvent-community-authentication.yml
summary_line: openIdConnect/oauth2/saml2 · 2 schemes
tags:
- Certification
- Community
- Customer-Support
- Cvent Academy
- Education
- Forums
- Knowledge Base
- Learning Centers
- Software-as-a-Service
- Training
---
