---
api_key_in:
- header
auth_types:
- http
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dataloop Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: DataLoop secures its APIs with http, oauth2, and apiKey across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: DataLoop
provider_slug: dataloop
scheme_count: 5
schemes:
- bearerFormat: JWT
  description: Every request to the Dataloop platform API carries a JWT in the Authorization header as a bearer token. This is the single transport for all authenticated calls to https://gate.dataloop.ai/api/v1.
  in: header
  name: BearerJWT
  parameter: Authorization
  scheme: bearer
  source: https://docs.dataloop.ai/docs/rest-api-connection
  type: http
- constraints:
    expiration: 1 year
    max_keys_per_project: 10
    max_keys_per_user: 10
    revocation: A Developer can revoke their own keys and list all keys in the project; a project Owner can revoke any key in the project.
  description: Dataloop API keys are JSON Web Tokens tied to a platform user and inherit that user's permissions. Generated from the project Dashboard; visible only once at creation. Only users with the Developer role or higher can create keys.
  format: JWT
  in: header
  name: APIKey
  parameter: Authorization
  source: https://docs.dataloop.ai/docs/rest-api-connection
  type: apiKey
- description: Exchange registered account credentials for a JWT. Documented for external systems (Postman/Insomnia) that need a bearer token. Google-SSO accounts must have a password set and log in once before this flow works.
  flow: password-style token exchange
  name: UserCredentialsToken
  request:
    body_fields:
    - username
    - password
    - type
    content_type: application/json
    method: POST
    type_value: user_credentials
  source: https://docs.dataloop.ai/docs/rest-api-connection
  token_endpoint: https://gate.dataloop.ai/token?default
  type: oauth2
- cli: dlp login-m2m -e <email> -p <password> -i <client-id> -s <client-secret>
  credentials:
  - client_id
  - client_secret
  - email
  - password
  description: Machine-to-machine login for long-running SDK jobs and automation. Exposed by the first-party CLI as `dlp login-m2m` / `dlp login-secret`, and by the SDK as the recommended path for running API commands from an external system.
  flow: clientCredentials
  identity_provider: Auth0
  name: M2M
  source: https://sdk-docs.dataloop.ai/en/latest/cli.html
  type: oauth2
- cli: dlp login
  description: Interactive browser login through the Auth0 hosted interface, used by the SDK and CLI for developer sessions. `dlp login-token -t <token>` accepts a previously obtained JWT.
  flow: authorizationCode
  identity_provider: Auth0
  name: InteractiveLogin
  source: https://sdk-docs.dataloop.ai/en/latest/cli.html
  type: oauth2
slug: dataloop-authentication
source_filename: dataloop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://docs.dataloop.ai/docs/rest-api-connection\ndocs: https://docs.dataloop.ai/docs/rest-api-connection\nnotes: >-\n  Dataloop publishes no public OpenAPI, so this profile is captured from the\n  provider's own API Authentication documentation and from the first-party\n  Python SDK/CLI (dtlpy), not derived from securitySchemes.\nsummary:\n  types: [http, oauth2, apiKey]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  oauth2_flows: [clientCredentials, authorizationCode]\n  identity_provider: Auth0\nschemes:\n- name: BearerJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter: Authorization\n  description: >-\n    Every request to the Dataloop platform API carries a JWT in the Authorization\n    header as a bearer token. This is the single transport for all authenticated\n    calls to https://gate.dataloop.ai/api/v1.\n  source: https://docs.dataloop.ai/docs/rest-api-connection\n\
  - name: APIKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: JWT\n  description: >-\n    Dataloop API keys are JSON Web Tokens tied to a platform user and inherit that\n    user's permissions. Generated from the project Dashboard; visible only once at\n    creation. Only users with the Developer role or higher can create keys.\n  constraints:\n    max_keys_per_user: 10\n    max_keys_per_project: 10\n    expiration: 1 year\n    revocation: >-\n      A Developer can revoke their own keys and list all keys in the project;\n      a project Owner can revoke any key in the project.\n  source: https://docs.dataloop.ai/docs/rest-api-connection\n- name: UserCredentialsToken\n  type: oauth2\n  flow: password-style token exchange\n  token_endpoint: https://gate.dataloop.ai/token?default\n  request:\n    method: POST\n    content_type: application/json\n    body_fields: [username, password, type]\n    type_value: user_credentials\n  description: >-\n    Exchange registered account\
  \ credentials for a JWT. Documented for external\n    systems (Postman/Insomnia) that need a bearer token. Google-SSO accounts must\n    have a password set and log in once before this flow works.\n  source: https://docs.dataloop.ai/docs/rest-api-connection\n- name: M2M\n  type: oauth2\n  flow: clientCredentials\n  identity_provider: Auth0\n  credentials: [client_id, client_secret, email, password]\n  cli: dlp login-m2m -e <email> -p <password> -i <client-id> -s <client-secret>\n  description: >-\n    Machine-to-machine login for long-running SDK jobs and automation. Exposed by\n    the first-party CLI as `dlp login-m2m` / `dlp login-secret`, and by the SDK as\n    the recommended path for running API commands from an external system.\n  source: https://sdk-docs.dataloop.ai/en/latest/cli.html\n- name: InteractiveLogin\n  type: oauth2\n  flow: authorizationCode\n  identity_provider: Auth0\n  cli: dlp login\n  description: >-\n    Interactive browser login through the Auth0 hosted interface,\
  \ used by the SDK\n    and CLI for developer sessions. `dlp login-token -t <token>` accepts a\n    previously obtained JWT.\n  source: https://sdk-docs.dataloop.ai/en/latest/cli.html\nauthorization_model:\n  style: role-based\n  docs: https://docs.dataloop.ai/docs/roles-and-permissions\n  note: >-\n    Dataloop does not publish an OAuth scope registry. Access is governed by\n    organization/project roles (Owner, Developer, Annotator, Annotation Manager\n    and organization-level roles) that the JWT inherits from its user, so there is\n    no scopes/ artifact for this provider.\ngap:\n  summary: >-\n    Authentication is documented in prose only. There is no machine-readable\n    securityScheme (no public OpenAPI), no OIDC discovery document, and no\n    /.well-known/oauth-authorization-server, so an agent cannot negotiate auth\n    programmatically — it must read the docs page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dataloop/refs/heads/main/authentication/dataloop-authentication.yml
summary_line: http/oauth2/apiKey · 5 schemes
tags:
- Artificial Intelligence
- Machine-Learning
- Data Management
- Data Annotation
- MLOps
- Computer-Vision
- Generative AI
- Data Labeling
- Pipelines
- Serverless
- Enterprise Software
- Company
---
