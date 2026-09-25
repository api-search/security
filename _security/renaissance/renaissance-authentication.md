---
anonymous_access: false
api_key_in: []
api_specs:
- filename: renaissance-lexile-api-openapi.yml
  format: yaml
  label: Lexile API
  slug: lexile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-lexile-api-openapi.yml
- filename: renaissance-classes-api-openapi.yml
  format: yaml
  label: Renaissance Classes API
  slug: renaissance-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-classes-api-openapi.yml
- filename: renaissance-events-api-openapi.yml
  format: yaml
  label: Renaissance Events API
  slug: renaissance-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-events-api-openapi.yml
- filename: renaissance-health-api-openapi.yml
  format: yaml
  label: Renaissance Health API
  slug: renaissance-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-health-api-openapi.yml
- filename: renaissance-pathway-api-openapi.yml
  format: yaml
  label: Renaissance Pathway API
  slug: renaissance-pathway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-pathway-api-openapi.yml
- filename: renaissance-predictions-api-openapi.yml
  format: yaml
  label: Renaissance Predictions API
  slug: renaissance-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-predictions-api-openapi.yml
- filename: renaissance-reading-level-api-openapi.yml
  format: yaml
  label: Renaissance Reading Level API
  slug: renaissance-reading-level-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-reading-level-api-openapi.yml
- filename: renaissance-skills-api-openapi.yml
  format: yaml
  label: Renaissance Skills API
  slug: renaissance-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-skills-api-openapi.yml
- filename: renaissance-utility-api-openapi.yml
  format: yaml
  label: Renaissance Utility API
  slug: renaissance-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-utility-api-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Renaissance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Renaissance secures its APIs with http, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Renaissance
provider_slug: renaissance
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT from Renaissance auth (client credentials). Token URL https://auth.stage.renaissance.com/oauth2/token (non-prod) or https://auth.renaissance.com/oauth2/token (prod). Request scope ren.lexile.read; the audience must match the API URL. Quoted verbatim from the Lexile API securityScheme description.
  enforced_by: API Gateway
  name: Bearer
  scheme: bearer
  scope_required: ren.lexile.read
  sources:
  - openapi/renaissance-lexile-api-openapi.yml
  type: http
- description: HTTP bearer scheme applied to every scored operation of the Student Proficiency Service and the Student Pathway Event Proxy. The specs declare no bearerFormat and no flows; the issuer is established by the authorization server above, not by the spec.
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/renaissance-student-proficiency-service-openapi.yml
  - openapi/renaissance-student-pathway-event-proxy-openapi.yml
  type: http
slug: renaissance-authentication
source_filename: renaissance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://auth.renaissance.com/.well-known/openid-configuration\ndocs: https://auth.renaissance.com/.well-known/openid-configuration\nsummary:\n  types:\n    - http\n    - oauth2\n    - openIdConnect\n  model: >-\n    Every Renaissance API contract found declares a single HTTP bearer JWT scheme. The tokens are\n    issued by Renaissance's own OAuth 2.0 / OpenID Connect authorization server at\n    auth.renaissance.com, which serves a live discovery document and JWKS. The Lexile API's\n    securityScheme description names the token endpoint and grant explicitly (client credentials),\n    which is what ties the spec-level bearer scheme to the authorization server.\nauthorization_server:\n  issuer: https://auth.renaissance.com\n  discovery: https://auth.renaissance.com/.well-known/openid-configuration\n  oauth_authorization_server: https://auth.renaissance.com/.well-known/oauth-authorization-server\n  http_status: 200\n  software:\
  \ Ory Hydra (identified by the credentials_endpoint_draft_00 / credentials_supported_draft_00 keys)\n  authorization_endpoint: https://auth.renaissance.com/oauth2/auth\n  token_endpoint: https://auth.renaissance.com/oauth2/token\n  device_authorization_endpoint: https://auth.renaissance.com/oauth2/device/auth\n  userinfo_endpoint: https://auth.renaissance.com/userinfo\n  revocation_endpoint: https://auth.renaissance.com/oauth2/revoke\n  end_session_endpoint: https://auth.renaissance.com/oauth2/sessions/logout\n  jwks_uri: https://auth.renaissance.com/.well-known/jwks.json\n  grant_types_supported:\n    - authorization_code\n    - implicit\n    - client_credentials\n    - refresh_token\n    - urn:ietf:params:oauth:grant-type:device_code\n  token_endpoint_auth_methods_supported:\n    - client_secret_post\n    - client_secret_basic\n    - private_key_jwt\n    - none\n  code_challenge_methods_supported:\n    - plain\n    - S256\n  id_token_signing_alg_values_supported:\n    - RS256\n  scopes_supported:\n\
  \    - openid\n    - offline\n    - offline_access\n  non_prod_token_endpoint: https://auth.stage.renaissance.com/oauth2/token\nschemes:\n  - name: Bearer\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      JWT from Renaissance auth (client credentials). Token URL\n      https://auth.stage.renaissance.com/oauth2/token (non-prod) or\n      https://auth.renaissance.com/oauth2/token (prod). Request scope ren.lexile.read; the audience\n      must match the API URL. Quoted verbatim from the Lexile API securityScheme description.\n    scope_required: ren.lexile.read\n    enforced_by: API Gateway\n    sources:\n      - openapi/renaissance-lexile-api-openapi.yml\n  - name: HTTPBearer\n    type: http\n    scheme: bearer\n    description: >-\n      HTTP bearer scheme applied to every scored operation of the Student Proficiency Service and the\n      Student Pathway Event Proxy. The specs declare no bearerFormat and no flows; the issuer is\n      established by\
  \ the authorization server above, not by the spec.\n    sources:\n      - openapi/renaissance-student-proficiency-service-openapi.yml\n      - openapi/renaissance-student-pathway-event-proxy-openapi.yml\nunauthenticated_operations:\n  - operationId: health_check_health_get\n    path: /health\n    api: Student Proficiency Service\n  - operationId: launch_launch_post\n    path: /launch\n    api: Student Proficiency Service\n  - operationId: health_health_get\n    path: /health\n    api: Student Pathway Event Proxy\nother_identity_surfaces:\n  - name: Renaissance Support community (Salesforce Experience Cloud)\n    issuer: https://support.renaissance.com\n    discovery: https://support.renaissance.com/.well-known/openid-configuration\n    http_status: 200\n    note: >-\n      Salesforce-provided OIDC surface running under a Renaissance-controlled host. It authenticates\n      the support community, not the product APIs, and its scopes_supported list is Salesforce's\n      stock platform set.\n\
  \  - name: Single sign-on for districts\n    note: >-\n      Renaissance product sign-in supports Google, Microsoft and Clever SSO plus SAML; recorded from\n      the provider's support material, not probed.\nprobe_evidence:\n  - url: https://auth.renaissance.com/.well-known/openid-configuration\n    status: 200\n  - url: https://auth.renaissance.com/.well-known/jwks.json\n    status: 200\n  - url: https://api.proxile.renaissance.com/api/lexile/9780439064873\n    status: 401\n    note: anonymous call to a real operation returns 401, confirming the gate is live\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/authentication/renaissance-authentication.yml
summary_line: http/oauth2/openIdConnect · 2 schemes
tags:
- Education
- EdTech
- K-12
- Assessment
- Learning Analytics
- Student Data
- OneRoster
- LTI
- Ed-Fi
- Rostering
- Interoperability
- Machine Learning
---
