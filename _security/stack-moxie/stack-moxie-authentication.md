---
api_key_in: []
api_specs:
- filename: stack-moxie-rest-api-openapi.yml
  format: yaml
  label: Stack Moxie REST API
  slug: stack-moxie-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-moxie/refs/heads/main/openapi/stack-moxie-rest-api-openapi.yml
auth_types:
- http
- grpc-metadata
- saml
description: ''
kind: authentication
layout: security
method: searched
name: Stack Moxie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stack Moxie secures its APIs with http, grpc-metadata, and saml across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Stack Moxie
provider_slug: stack-moxie
scheme_count: 3
schemes:
- applies_to: Stack Moxie REST API (all operations)
  bearerFormat: JWT
  expiry: not documented
  header: 'Authorization: Bearer <jwt>'
  name: jwtBearerAuth
  rotation: not documented
  scheme: bearer
  scope_model: 'Authorization is organization-scoped by path, not by token scope - every operation is nested under /v1/organizations/{org} where {org} is the Organization UUID. Two distinct failure responses distinguish the cases: 401 Unauthorized ("there may be a problem with your API token") and 403 Forbidden ("the authenticated user isn''t allowed to perform this action").'
  scoped: false
  security_applied: global
  security_applied_detail: 'Declared once at the document root as `security: [{jwtBearerAuth: []}]`, so every operation inherits it; no operation opts out and there is no anonymous endpoint.'
  sources:
  - openapi/stack-moxie-rest-api-openapi.yml
  token_management: '"You can manage your API tokens on your account settings page" - tokens are issued and revoked in the app UI at https://app.stackmoxie.com; there is no token, refresh or introspection endpoint in the API itself.'
  type: http
- applies_to: Crank Cogs (open-source, self-run)
  credential_carrier: gRPC call metadata
  description: Each Cog self-declares the credentials it needs by returning a CogManifest.auth_fields list (repeated FieldDefinition) from the GetManifest RPC. Every FieldDefinition carries a key, a type (STRING, BOOLEAN, NUMERIC, DATE, DATETIME, EMAIL, PHONE, URL, MAP, ANYSCALAR, ANYNONSCALAR), an optionality (OPTIONAL | REQUIRED), and help text. The client (crank) collects those values and sets each as gRPC call metadata, keyed by the FieldDefinition key, on every RunStep / RunSteps call.
  discovery_operation: GetManifest
  field_key_example: mySystemAuthToken
  help_url_field: CogManifest.auth_help_url
  hosted_equivalent: In the hosted product the same credentials are stored as a Connection (POST /v1/organizations/{org}/connections) whose write-only `auth` object holds the Cog's auth fields and whose `isValid` flag reports whether they still work. The Cog registry those fields belong to is readable at GET /v1/organizations/{org}/registry, which returns RegistryEntry objects carrying authFieldsList and authHelpUrl - the REST projection of CogManifest.
  name: CogAuthFields
  protocol: gRPC (proto3), automaton.cog.CogService
  sources:
  - grpc/stack-moxie-cog.proto
  type: grpc-metadata
- applies_to: Stack Moxie web application (human login, not API)
  name: Hosted app SSO
  plans:
    Enterprise: SSO (Federated or SAML)
    Growth: SSO (SAML)
    Individual: none
    Starter: none
  source: https://www.stackmoxie.com/pricing/
  type: saml
slug: stack-moxie-authentication
source_filename: stack-moxie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/stack-moxie-rest-api-openapi.yml\ndocs: https://api.stackmoxie.com/#section/Authentication\nnote: >-\n  Two separate authentication models exist and they are easy to confuse. The\n  hosted Stack Moxie REST API uses HTTP Bearer with a JWT you manage on your\n  account settings page, applied globally to all 43 operations. The open-source\n  Cog gRPC contract uses per-Cog credentials passed as gRPC call metadata, and\n  those credentials authenticate a Cog to the THIRD-PARTY SYSTEM UNDER TEST, not\n  to Stack Moxie. Both are captured below.\nsummary:\n  types:\n  - http\n  - grpc-metadata\n  - saml\n  api_key_in: []\n  oauth2_flows: []\n  public_api: true\nschemes:\n- name: jwtBearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: Stack Moxie REST API (all operations)\n  sources:\n  - openapi/stack-moxie-rest-api-openapi.yml\n  security_applied: global\n  security_applied_detail: >-\n    Declared\
  \ once at the document root as `security: [{jwtBearerAuth: []}]`, so\n    every operation inherits it; no operation opts out and there is no anonymous\n    endpoint.\n  token_management: >-\n    \"You can manage your API tokens on your account settings page\" - tokens are\n    issued and revoked in the app UI at https://app.stackmoxie.com; there is no\n    token, refresh or introspection endpoint in the API itself.\n  header: 'Authorization: Bearer <jwt>'\n  scoped: false\n  scope_model: >-\n    Authorization is organization-scoped by path, not by token scope - every\n    operation is nested under /v1/organizations/{org} where {org} is the\n    Organization UUID. Two distinct failure responses distinguish the cases:\n    401 Unauthorized (\"there may be a problem with your API token\") and\n    403 Forbidden (\"the authenticated user isn't allowed to perform this action\").\n  expiry: not documented\n  rotation: not documented\n- name: CogAuthFields\n  type: grpc-metadata\n  protocol:\
  \ gRPC (proto3), automaton.cog.CogService\n  applies_to: Crank Cogs (open-source, self-run)\n  sources:\n  - grpc/stack-moxie-cog.proto\n  description: >-\n    Each Cog self-declares the credentials it needs by returning a\n    CogManifest.auth_fields list (repeated FieldDefinition) from the GetManifest\n    RPC. Every FieldDefinition carries a key, a type (STRING, BOOLEAN, NUMERIC,\n    DATE, DATETIME, EMAIL, PHONE, URL, MAP, ANYSCALAR, ANYNONSCALAR), an\n    optionality (OPTIONAL | REQUIRED), and help text. The client (crank) collects\n    those values and sets each as gRPC call metadata, keyed by the FieldDefinition\n    key, on every RunStep / RunSteps call.\n  discovery_operation: GetManifest\n  credential_carrier: gRPC call metadata\n  field_key_example: mySystemAuthToken\n  help_url_field: CogManifest.auth_help_url\n  hosted_equivalent: >-\n    In the hosted product the same credentials are stored as a Connection\n    (POST /v1/organizations/{org}/connections) whose write-only `auth`\
  \ object\n    holds the Cog's auth fields and whose `isValid` flag reports whether they\n    still work. The Cog registry those fields belong to is readable at\n    GET /v1/organizations/{org}/registry, which returns RegistryEntry objects\n    carrying authFieldsList and authHelpUrl - the REST projection of CogManifest.\n- name: Hosted app SSO\n  type: saml\n  applies_to: Stack Moxie web application (human login, not API)\n  source: https://www.stackmoxie.com/pricing/\n  plans:\n    Starter: none\n    Individual: none\n    Growth: SSO (SAML)\n    Enterprise: SSO (Federated or SAML)\ngaps:\n- no OAuth 2.0 or OpenID Connect surface; /.well-known/oauth-authorization-server\n  and /.well-known/openid-configuration return 404 on every host\n- no token endpoint, no refresh flow, no introspection or revocation endpoint in\n  the API - token lifecycle is entirely a UI operation\n- no documented token expiry or rotation policy\n- no scopes; authorization is coarse, by organization membership and\
  \ role\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stack-moxie/refs/heads/main/authentication/stack-moxie-authentication.yml
summary_line: http/grpc-metadata/saml · 3 schemes
tags:
- Company
- RevOps
- Marketing Operations
- Observability
- Monitoring
- Testing
- Test Automation
- QA Automation
- Marketing Automation
- Email Deliverability
- Salesforce
- Marketo
- gRPC
- SaaS
---
