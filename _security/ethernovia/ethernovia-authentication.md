---
api_key_in: []
api_specs:
- filename: ethernovia-audit-user-trail-api-openapi.yml
  format: yaml
  label: Ethernovia Audit User Trail API
  slug: ethernovia-audit-user-trail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-audit-user-trail-api-openapi.yml
- filename: ethernovia-ec-document-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Document API
  slug: ethernovia-ec-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-document-api-openapi.yml
- filename: ethernovia-ec-document-type-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Document Type API
  slug: ethernovia-ec-document-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-document-type-api-openapi.yml
- filename: ethernovia-ec-excluded-domain-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Excluded Domain API
  slug: ethernovia-ec-excluded-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-excluded-domain-api-openapi.yml
- filename: ethernovia-ec-group-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Group API
  slug: ethernovia-ec-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-group-api-openapi.yml
- filename: ethernovia-ec-product-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Product API
  slug: ethernovia-ec-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-product-api-openapi.yml
- filename: ethernovia-ec-product-category-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Product Category API
  slug: ethernovia-ec-product-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-product-category-api-openapi.yml
- filename: ethernovia-ec-product-family-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Product Family API
  slug: ethernovia-ec-product-family-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-product-family-api-openapi.yml
- filename: ethernovia-ec-send-alert-email-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Send Alert Email API
  slug: ethernovia-ec-send-alert-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-send-alert-email-api-openapi.yml
- filename: ethernovia-ec-software-package-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Software Package API
  slug: ethernovia-ec-software-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-software-package-api-openapi.yml
- filename: ethernovia-ec-status-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Status API
  slug: ethernovia-ec-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-status-api-openapi.yml
- filename: ethernovia-my-download-api-openapi.yml
  format: yaml
  label: Ethernovia My Download API
  slug: ethernovia-my-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-my-download-api-openapi.yml
- filename: ethernovia-upload-file-api-openapi.yml
  format: yaml
  label: Ethernovia Upload - File API
  slug: ethernovia-upload-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-upload-file-api-openapi.yml
- filename: ethernovia-users-permissions-auth-api-openapi.yml
  format: yaml
  label: Ethernovia Users-Permissions - Auth API
  slug: ethernovia-users-permissions-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-users-permissions-auth-api-openapi.yml
- filename: ethernovia-users-permissions-users-roles-api-openapi.yml
  format: yaml
  label: Ethernovia Users-Permissions - Users & Roles API
  slug: ethernovia-users-permissions-users-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-users-permissions-users-roles-api-openapi.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Ethernovia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ethernovia secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ethernovia
provider_slug: ethernovia
scheme_count: 2
schemes:
- applied: global (root-level security requirement)
  bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ethernovia-customer-portal-openapi.yml
  type: http
- authorization_endpoint: https://ethernovia.us.auth0.com/authorize
  code_challenge_methods_supported:
  - S256
  - plain
  entry_point: https://portal-admin.ethernovia.com/api/connect/auth0
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://ethernovia.us.auth0.com/
  jwks_uri: https://ethernovia.us.auth0.com/.well-known/jwks.json
  method: searched
  name: auth0
  openIdConnectUrl: https://ethernovia.us.auth0.com/.well-known/openid-configuration
  scopes_supported:
  - openid
  - profile
  - offline_access
  - name
  - given_name
  - family_name
  - nickname
  - email
  - email_verified
  - picture
  - created_at
  - identities
  - phone
  - address
  sources:
  - well-known/ethernovia-auth0-openid-configuration.json
  token_endpoint: https://ethernovia.us.auth0.com/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://ethernovia.us.auth0.com/userinfo
slug: ethernovia-authentication
source_filename: ethernovia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/ethernovia-customer-portal-openapi.yml\ndocs: https://portal-admin.ethernovia.com/documentation\nsummary:\n  types:\n  - http\n  - openIdConnect\n  http_schemes:\n  - bearer\n  bearer_formats:\n  - JWT\n  identity_provider: Auth0 (ethernovia.us.auth0.com)\n  anonymous_access: false\n  note: >-\n    Every data endpoint on the Customer Portal API is bearer-JWT protected and returns\n    HTTP 403 ForbiddenError anonymously (verified 2026-08-04). Interactive sign-in is\n    federated to the company's Auth0 tenant; the Strapi users-permissions plugin also\n    exposes local email/password auth endpoints (/auth/local, /auth/local/register).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied: global (root-level security requirement)\n  sources:\n  - openapi/ethernovia-customer-portal-openapi.yml\n- name: auth0\n  type: openIdConnect\n  method: searched\n  openIdConnectUrl: https://ethernovia.us.auth0.com/.well-known/openid-configuration\n\
  \  issuer: https://ethernovia.us.auth0.com/\n  authorization_endpoint: https://ethernovia.us.auth0.com/authorize\n  token_endpoint: https://ethernovia.us.auth0.com/oauth/token\n  userinfo_endpoint: https://ethernovia.us.auth0.com/userinfo\n  jwks_uri: https://ethernovia.us.auth0.com/.well-known/jwks.json\n  entry_point: https://portal-admin.ethernovia.com/api/connect/auth0\n  scopes_supported: [openid, profile, offline_access, name, given_name, family_name,\n    nickname, email, email_verified, picture, created_at, identities, phone, address]\n  grant_types_supported: [authorization_code, client_credentials, refresh_token, implicit,\n    password, 'urn:ietf:params:oauth:grant-type:device_code', 'urn:ietf:params:oauth:grant-type:token-exchange',\n    'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  code_challenge_methods_supported: [S256, plain]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post,\n    private_key_jwt, none]\n  sources:\n  - well-known/ethernovia-auth0-openid-configuration.json\n\
  local_auth_operations:\n- POST /auth/local\n- POST /auth/local/register\n- POST /auth/forgot-password\n- POST /auth/reset-password\n- POST /auth/change-password\n- GET /auth/{provider}/callback\n- GET /connect/{provider}\ngated_developer_surface:\n  note: >-\n    Ethernovia's product-facing software — tools, software binaries, source-code drivers,\n    header files and plug-in APIs, plus their documentation — is not reachable anonymously.\n    Access is granted through the Customer Portal under an NDA, and use is governed by a\n    separate EULA that accompanies the software rather than by the public Terms of Use.\n  source: https://www.ethernovia.com/terms-of-use/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/authentication/ethernovia-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- Company
- Semiconductors
- Automotive
- Ethernet
- Networking
- Hardware
- Robotics
- Artificial Intelligence
- Autonomous Vehicles
- Physical AI
---
