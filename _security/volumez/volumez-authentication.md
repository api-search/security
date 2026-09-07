---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: volumez-orchestrator-api-openapi.yaml
  format: yaml
  label: Volumez Orchestrator API
  slug: volumez-orchestrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volumez/refs/heads/main/openapi/volumez-orchestrator-api-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Volumez Authentication
name_suffix: Authentication
oauth_flows: []
overview: Volumez secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Volumez
provider_slug: volumez
scheme_count: 1
schemes:
- description: 'Every protected operation takes a JWT in the `authorization` request header. The OpenAPI declares this as an apiKey-in-header scheme carrying the AWS API Gateway extension x-amazon-apigateway-authtype: cognito_user_pools, so the token is validated against a Cognito user pool (providerARN arn:aws:cognito-idp:us-east-1:...:userpool/us-east-1_Mk5LdUo2I) rather than by a bespoke key store. 108 of the 124 operations declare it; 16 are unauthenticated (signin, signup, password reset, SSO callback, the public infra planner and the version endpoint).'
  in: header
  name: storage.io-authorizer
  parameter: authorization
  sources:
  - openapi/volumez-orchestrator-api-openapi.yaml
  type: apiKey
slug: volumez-authentication
source_filename: volumez-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  openapi/volumez-orchestrator-api-openapi.yaml (components.securitySchemes) enriched from the\n  provider's own \"Sign In and Authentication\", \"API\" and \"User and Token Management\" documentation\n  pages, which are no longer reachable live (docs.volumez.com serves no valid TLS certificate) and\n  were read from the Internet Archive captures of docs.volumez.com/docs/authentication,\n  /docs/api-1 and /docs/user-and-token-management.\ndocs: https://web.archive.org/web/2025/https://docs.volumez.com/docs/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  identity_provider: AWS Cognito user pool\n  token_format: JWT\nschemes:\n- name: storage.io-authorizer\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: >-\n    Every protected operation takes a JWT in the `authorization` request header. The OpenAPI declares\n    this as an apiKey-in-header scheme carrying the AWS API Gateway\
  \ extension\n    x-amazon-apigateway-authtype: cognito_user_pools, so the token is validated against a Cognito user\n    pool (providerARN arn:aws:cognito-idp:us-east-1:...:userpool/us-east-1_Mk5LdUo2I) rather than by a\n    bespoke key store. 108 of the 124 operations declare it; 16 are unauthenticated (signin, signup,\n    password reset, SSO callback, the public infra planner and the version endpoint).\n  sources:\n  - openapi/volumez-orchestrator-api-openapi.yaml\ntoken_exchange:\n  operation: signIn\n  endpoint: POST /signin\n  documented_host: https://api.volumez.com\n  request:\n    content_type: application/json\n    body: '{ \"email\": \"string\", \"password\": \"string\" }'\n  response_fields:\n  - {name: AccessToken, type: string, description: Token used for accessing protected routes.}\n  - {name: IdToken, type: string, description: JWT carrying user identity; this is the value the provider's own examples put in the authorization header.}\n  - {name: RefreshToken, type: string,\
  \ description: Token used to obtain new access tokens.}\n  - {name: ExpiresIn, type: number, description: Token lifetime in seconds (86400 in the published sample).}\n  - {name: TokenType, type: string, description: 'Bearer'}\n  note: >-\n    The provider's own curl samples send the raw IdToken as the `authorization` header value with no\n    \"Bearer \" prefix. The generated Go client README instead sets `Authorization: Bearer <token>`.\n    Both forms appear in first-party material; an integrator should expect the raw-JWT form the\n    documentation samples use.\ntoken_types:\n  - name: Volumez REST API Token (JWT Identity Token)\n    use: Public REST API calls.\n  - name: Tenant Token (JWT Access Token)\n    use: Used by a Volumez Connector; identifies the tenant. Also the `tenant_token` Terraform input.\n  - name: Tenant Host Token / Refresh Token (JWT Refresh Token)\n    use: Used by a Volumez Connector; identifies the tenant's host.\n  - name: CSI Driver Token (Refresh Token)\n \
  \   use: Passed to the Kubernetes CSI driver as helm value `vlzAuthToken`. Documented to expire in 10 years.\ntoken_types_source: https://web.archive.org/web/2025/https://docs.volumez.com/docs/api-1\nissuance:\n  self_serve: true\n  path: >-\n    POST /signup registers an account; tokens are then read from the Volumez portal under\n    DEVELOPER > Developer Info. As of 2026-09-04 the portal, the API host (api.volumez.com) and the\n    documentation host are no longer resolvable/serving, so no new credential can be obtained.\nrelated_operations:\n  signin: signIn\n  signout: signOut\n  signup: SignUp\n  refresh: getTenantRefreshToken\n  tenant_access_token: getTenantAccessToken\n  rotate_api_credentials: RefreshTenantAPIAccessCredentials\n  change_password: [requestChangePassword, approveChangePassword, ChangePasswordLoggedIn]\n  sso: [putAzureSSOMapping, getAzureSSOMapping, deleteAzureSSOMapping, handleSSOCallback]\nsso:\n  supported: true\n  providers: [Azure Active Directory / Entra\
  \ ID]\n  operations: [putAzureSSOMapping, getAzureSSOMapping, deleteAzureSSOMapping, handleSSOCallback]\n  docs: https://web.archive.org/web/2025/https://docs.volumez.com/docs/azure-active-directory-ad\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volumez/refs/heads/main/authentication/volumez-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Storage
- Block Storage
- Data Infrastructure
- Cloud Infrastructure
- Kubernetes
- Container Storage Interface
- AI Infrastructure
- Snapshots
- Infrastructure as Code
- DIaaS
---
