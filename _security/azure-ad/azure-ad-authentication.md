---
anonymous_access: false
api_key_in: []
api_specs:
- filename: azure-ad-graph-applications-openapi.yml
  format: yaml
  label: Azure Active Directory Applications API
  slug: azure-ad-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-applications-openapi.yml
- filename: azure-ad-graph-identity-directorymanagement-openapi.yml
  format: yaml
  label: Azure Active Directory Directory API
  slug: azure-ad-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-identity-directorymanagement-openapi.yml
- filename: azure-ad-graph-groups-openapi.yml
  format: yaml
  label: Azure Active Directory Groups API
  slug: azure-ad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-groups-openapi.yml
- filename: azure-ad-me-api-openapi.yml
  format: yaml
  label: Azure Active Directory Me API
  slug: azure-ad-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/azure-ad-me-api-openapi.yml
- filename: azure-ad-graph-users-openapi.yml
  format: yaml
  label: Azure Active Directory Users API
  slug: azure-ad-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-users-openapi.yml
- filename: azure-ad-graph-identity-signins-openapi.yml
  format: yaml
  label: Microsoft Entra ID Sign-Ins and Policies API
  slug: azure-ad-signins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-identity-signins-openapi.yml
- filename: azure-ad-graph-identity-governance-openapi.yml
  format: yaml
  label: Microsoft Entra ID Governance API
  slug: azure-ad-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-identity-governance-openapi.yml
- filename: azure-ad-graph-directoryobjects-openapi.yml
  format: yaml
  label: Microsoft Entra ID Directory Objects API
  slug: azure-ad-directory-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-directoryobjects-openapi.yml
- filename: azure-ad-graph-changenotifications-openapi.yml
  format: yaml
  label: Microsoft Entra ID Change Notifications API
  slug: azure-ad-change-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-changenotifications-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Azure Ad Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
overview: Microsoft Entra ID (formerly Azure AD) secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and deviceCode flow(s).
provider_name: Microsoft Entra ID (formerly Azure AD)
provider_slug: azure-ad
scheme_count: 3
schemes:
- applied: global `security` requirement on each document
  declared_in: every spec in openapi/_original/azure-ad-graph-*.yml
  description: Microsoft identity platform v2.0 (Microsoft Entra ID)
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
    description: The app acts on behalf of a signed-in user. Effective access is the INTERSECTION of the granted scope and the user's own directory privileges — a token carrying User.ReadWrite.All still cannot edit a user the signed-in principal has no rights over.
    flow: authorizationCode
    permission_set: delegated
    pkce: required for public clients
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  - client_authentication:
    - client_secret_post
    - client_secret_basic
    - private_key_jwt
    - self_signed_tls_client_auth
    description: The app acts as itself, with no user context. Admin consent is always required and access is tenant-wide, bounded only by the granted application permissions. This is the daemon/agent path.
    flow: clientCredentials
    note: token_endpoint_auth_methods_supported read verbatim from the discovery document. private_key_jwt (certificate credentials) and federated identity credentials are the recommended alternatives to a shared secret for unattended workloads.
    permission_set: application
    scope_parameter: https://graph.microsoft.com/.default
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  - description: RFC 8628 device authorization grant, for input-constrained clients.
    deviceAuthorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/devicecode
    flow: deviceCode
    permission_set: delegated
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: azureaadv2
  type: oauth2
- description: Full OpenID Connect provider. Discovery returns issuer https://login.microsoftonline.com/{tenantid}/v2.0, jwks_uri https://login.microsoftonline.com/common/discovery/v2.0/keys, userinfo at https://graph.microsoft.com/oidc/userinfo, RS256 id_token signing and pairwise subject identifiers.
  name: openIdConnect
  openIdConnectUrl: https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration
  type: openIdConnect
- description: self_signed_tls_client_auth is advertised in token_endpoint_auth_methods_supported — client certificates may authenticate at the token endpoint. Not a transport-level mTLS requirement on graph.microsoft.com itself.
  name: mutualTLS
  type: mutualTLS
slug: azure-ad-authentication
source_filename: azure-ad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://learn.microsoft.com/en-us/graph/auth/ ,\n  https://learn.microsoft.com/en-us/entra/identity-platform/v2-overview ,\n  https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration\n  (fetched 200, saved at well-known/azure-ad-openid-configuration.json), and the\n  azureaadv2 securityScheme declared in every harvested spec under\n  openapi/_original/\nprovider: Azure Active Directory (Microsoft Entra ID)\nproviderId: azure-ad\nsupersedes: >-\n  The 2026-07-11 derived file, whose endpoints came from a hand-written scaffold\n  spec rather than from the provider's own discovery document.\nsummary:\n  types:\n    - oauth2\n    - openIdConnect\n  oauth2_flows:\n    - authorizationCode\n    - clientCredentials\n    - deviceCode\n  api_keys: false\n  basic_auth: false\n  mtls: true\n  note: >-\n    Microsoft Graph accepts no API key and no basic auth. Every request carries an\n    OAuth 2.0 bearer token\
  \ issued by the Microsoft identity platform v2.0\n    endpoint. An anonymous request to graph.microsoft.com returns 401\n    InvalidAuthenticationToken — verified live on 2026-09-06.\nschemes:\n  - name: azureaadv2\n    type: oauth2\n    description: Microsoft identity platform v2.0 (Microsoft Entra ID)\n    declared_in: every spec in openapi/_original/azure-ad-graph-*.yml\n    applied: global `security` requirement on each document\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize\n        tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n        permission_set: delegated\n        pkce: required for public clients\n        description: >-\n          The app acts on behalf of a signed-in user. Effective access is the\n          INTERSECTION of the granted scope and the user's own directory\n          privileges — a token carrying User.ReadWrite.All still cannot edit a\n        \
  \  user the signed-in principal has no rights over.\n      - flow: clientCredentials\n        tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n        permission_set: application\n        scope_parameter: https://graph.microsoft.com/.default\n        description: >-\n          The app acts as itself, with no user context. Admin consent is always\n          required and access is tenant-wide, bounded only by the granted\n          application permissions. This is the daemon/agent path.\n        client_authentication:\n          - client_secret_post\n          - client_secret_basic\n          - private_key_jwt\n          - self_signed_tls_client_auth\n        note: >-\n          token_endpoint_auth_methods_supported read verbatim from the discovery\n          document. private_key_jwt (certificate credentials) and federated\n          identity credentials are the recommended alternatives to a shared\n          secret for unattended workloads.\n      - flow: deviceCode\n\
  \        deviceAuthorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/devicecode\n        tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n        permission_set: delegated\n        description: RFC 8628 device authorization grant, for input-constrained clients.\n  - name: openIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration\n    description: >-\n      Full OpenID Connect provider. Discovery returns issuer\n      https://login.microsoftonline.com/{tenantid}/v2.0, jwks_uri\n      https://login.microsoftonline.com/common/discovery/v2.0/keys, userinfo at\n      https://graph.microsoft.com/oidc/userinfo, RS256 id_token signing and\n      pairwise subject identifiers.\n  - name: mutualTLS\n    type: mutualTLS\n    description: >-\n      self_signed_tls_client_auth is advertised in\n      token_endpoint_auth_methods_supported — client certificates may\n      authenticate\
  \ at the token endpoint. Not a transport-level mTLS requirement\n      on graph.microsoft.com itself.\ntoken:\n  transport: 'Authorization: Bearer <token>'\n  format: JWT\n  signing_alg: RS256\n  jwks_uri: https://login.microsoftonline.com/common/discovery/v2.0/keys\n  audience: https://graph.microsoft.com\n  issuer_template: https://login.microsoftonline.com/{tenantid}/v2.0\n  subject_type: pairwise\n  claims_supported:\n    - sub\n    - iss\n    - aud\n    - exp\n    - iat\n    - auth_time\n    - acr\n    - nonce\n    - preferred_username\n    - name\n    - tid\n    - ver\n    - at_hash\n    - c_hash\n    - email\n    - cloud_instance_name\n    - cloud_instance_host_name\n    - cloud_graph_host_name\n    - msgraph_host\n  note: >-\n    Graph access tokens are opaque to third parties by contract — Microsoft\n    documents that only the resource may validate them, and the token format can\n    change. Do not parse a Graph access token in client code.\ntenant_segment:\n  values:\n    -\
  \ '{tenantId} — a single tenant'\n    - common — work, school or personal Microsoft accounts\n    - organizations — work or school accounts only\n    - consumers — personal Microsoft accounts only\n  note: >-\n    The tenant segment in the authority URL is part of the security boundary, not\n    a routing convenience. The Microsoft MCP Server for Enterprise names\n    https://login.microsoftonline.com/organizations/v2.0 specifically.\nauthorization:\n  model: OAuth scopes + directory roles + Conditional Access\n  scopes: scopes/azure-ad-scopes.yml\n  conditional_access_note: >-\n    A Conditional Access policy can refuse an otherwise valid token with\n    HTTP 403 and `error=insufficient_claims`. A client must handle the claims\n    challenge and re-authenticate; retrying the same token will never succeed.\n  docs: https://learn.microsoft.com/en-us/entra/identity-platform/v2-conditional-access-dev-guide\nverification:\n  probed: '2026-09-06'\n  anonymous_request: https://graph.microsoft.com/v1.0/users\n\
  \  http_status: 401\n  error_code: InvalidAuthenticationToken\ndocs: https://learn.microsoft.com/en-us/graph/auth/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/authentication/azure-ad-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Authentication
- Authorization
- Identity
- OpenID Connect
- Single Sign-On
---
