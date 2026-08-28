---
api_key_in:
- header
api_specs:
- filename: silverflow-openapi.yml
  format: yaml
  label: Silverflow API
  slug: silverflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverflow/refs/heads/main/openapi/silverflow-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Silverflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Silverflow secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Silverflow
provider_slug: silverflow
scheme_count: 3
schemes:
- bootstrap: The Agent Activation process (POST /v1/agents/{agentKey}/activate) mints the first API key from an Agent Activation Token issued during onboarding.
  credential_lifecycle: Created with POST /v1/apiKeys (createApiKey); up to 40 keys per agent; updatable and deletable, which is how credential rotation is done. The `secret` is returned ONCE, at creation, and is never retrievable again.
  description: 'The primary method of authenticating to the Silverflow API is through API keys.


    API keys can be created by calling the [createApiKey](#operation/createApiKey) endpoint. You can create up to 40 API keys and also update and delete them, allowing for _credential rotation_.


    The _Agent Activation_ process will generate an initial API Key for you. See [Activate Agent](#section/Getting-Started).


    A cal'
  name: ApiKey
  primary: true
  rfc: RFC 7617
  scheme: basic
  scoping:
    ip_restrictions: Keys can be pinned to CIDR ranges (e.g. 185.184.111.39/32, 102.177.115.120/29, 0.0.0.0/0). Use outside the range returns a generic 401 Authentication Required rather than a distinguishing error.
    permission_reference: https://docs.silverflow.com/apidocs/latest/index.html#tag/API-Keys/operation/createApiKey
    permissions: Each key carries an explicit permission list (e.g. charges:List, reports:All). A call lacking the permission returns 403 whose detail names the permission needed. Least privilege is documented as the recommended practice.
  sources:
  - openapi/silverflow-openapi.yml
  summary: HTTP Basic where username = API key `key` (prefix apk-) and password = the key `secret`.
  type: http
- bearerFormat: JWT
  credential_lifecycle: Created with POST /v1/agents/{agentKey}/bearerToken (createAgentBearerToken). Described as "temporary security credentials"; no published TTL.
  description: 'Bearer tokens are temporary security credentials that can be used to authorize ''third parties'' (bearers) access to the Silverflow API on behalf of the agent.


    These tokens are created by calling the [createAgentBearerToken](#operation/createAgentBearerToken) endpoint.


    Once created the `token` field must be used in the HTTP `Authorization` header using the `Bearer` scheme.

    Here''s an example of an '
  name: BearerToken
  primary: false
  rfc: RFC 6750
  scheme: bearer
  scoping:
    ip_restrictions: Supported, same CIDR mechanism.
    permissions: Same permission model as API keys.
  sources:
  - openapi/silverflow-openapi.yml
  summary: Short-lived JWT for delegating access to a third party on behalf of the agent.
  type: http
- actual_type: mutualTLS
  description: 'The client must set up mTLS connection with a valid X.509 client certificate signed by a customer-provided CA (certificate authority) that is registered to a specific agent. The customer-provided CA certificate must be shared and added to Silverflow''s trust store prior to calling endpoints.


    Certificate validation happens at the transport layer during TLS handshake. Tenant verification is performe'
  enrolment: The customer's CA certificate must be shared with Silverflow and added to its trust store before any call. Tenant verification matches the agent key embedded in the client certificate against the agent key embedded in the trusted CA.
  in: header
  name: MutualTLS
  parameter: '-'
  primary: false
  sources:
  - openapi/silverflow-openapi.yml
  summary: Transport-layer mTLS with an X.509 client certificate signed by a customer-provided CA registered against a specific agent.
  type: apiKey
  type_modelling_defect: 'Declared in the OpenAPI as `type: apiKey, in: header, name: ''-''` rather than OpenAPI 3.1''s `type: mutualTLS`. This is a spec-modelling workaround (OpenAPI 3.0.3 has no mutualTLS type), so a generator reading the spec will emit a bogus header parameter named ''-''. Worth reporting to Silverflow.'
  validation_point: TLS handshake
slug: silverflow-authentication
source_filename: silverflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://docs.silverflow.com/guides/authentication + openapi/silverflow-openapi.yml components.securitySchemes\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: http\n  scheme: basic\n  description: 'The primary method of authenticating to the Silverflow API is through API keys.\n\n\n    API keys can be created by calling the [createApiKey](#operation/createApiKey) endpoint. You can create\n    up to 40 API keys and also update and delete them, allowing for _credential rotation_.\n\n\n    The _Agent Activation_ process will generate an initial API Key for you. See [Activate Agent](#section/Getting-Started).\n\n\n    A cal'\n  sources:\n  - openapi/silverflow-openapi.yml\n  primary: true\n  summary: HTTP Basic where username = API key `key` (prefix apk-) and password = the key `secret`.\n  credential_lifecycle: Created with POST /v1/apiKeys (createApiKey); up to 40 keys per\
  \ agent; updatable\n    and deletable, which is how credential rotation is done. The `secret` is returned ONCE, at creation,\n    and is never retrievable again.\n  bootstrap: The Agent Activation process (POST /v1/agents/{agentKey}/activate) mints the first API key\n    from an Agent Activation Token issued during onboarding.\n  rfc: RFC 7617\n  scoping:\n    permissions: Each key carries an explicit permission list (e.g. charges:List, reports:All). A call\n      lacking the permission returns 403 whose detail names the permission needed. Least privilege is\n      documented as the recommended practice.\n    permission_reference: https://docs.silverflow.com/apidocs/latest/index.html#tag/API-Keys/operation/createApiKey\n    ip_restrictions: Keys can be pinned to CIDR ranges (e.g. 185.184.111.39/32, 102.177.115.120/29, 0.0.0.0/0).\n      Use outside the range returns a generic 401 Authentication Required rather than a distinguishing\n      error.\n- name: BearerToken\n  type: http\n  scheme:\
  \ bearer\n  bearerFormat: JWT\n  description: 'Bearer tokens are temporary security credentials that can be used to authorize ''third\n    parties'' (bearers) access to the Silverflow API on behalf of the agent.\n\n\n    These tokens are created by calling the [createAgentBearerToken](#operation/createAgentBearerToken)\n    endpoint.\n\n\n    Once created the `token` field must be used in the HTTP `Authorization` header using the `Bearer`\n    scheme.\n\n    Here''s an example of an '\n  sources:\n  - openapi/silverflow-openapi.yml\n  primary: false\n  summary: Short-lived JWT for delegating access to a third party on behalf of the agent.\n  credential_lifecycle: Created with POST /v1/agents/{agentKey}/bearerToken (createAgentBearerToken).\n    Described as \"temporary security credentials\"; no published TTL.\n  rfc: RFC 6750\n  scoping:\n    permissions: Same permission model as API keys.\n    ip_restrictions: Supported, same CIDR mechanism.\n- name: MutualTLS\n  type: apiKey\n  in:\
  \ header\n  parameter: '-'\n  description: 'The client must set up mTLS connection with a valid X.509 client certificate signed by\n    a customer-provided CA (certificate authority) that is registered to a specific agent. The customer-provided\n    CA certificate must be shared and added to Silverflow''s trust store prior to calling endpoints.\n\n\n    Certificate validation happens at the transport layer during TLS handshake. Tenant verification is\n    performe'\n  sources:\n  - openapi/silverflow-openapi.yml\n  primary: false\n  actual_type: mutualTLS\n  type_modelling_defect: 'Declared in the OpenAPI as `type: apiKey, in: header, name: ''-''` rather than\n    OpenAPI 3.1''s `type: mutualTLS`. This is a spec-modelling workaround (OpenAPI 3.0.3 has no mutualTLS\n    type), so a generator reading the spec will emit a bogus header parameter named ''-''. Worth reporting\n    to Silverflow.'\n  summary: Transport-layer mTLS with an X.509 client certificate signed by a customer-provided\
  \ CA registered\n    against a specific agent.\n  enrolment: The customer's CA certificate must be shared with Silverflow and added to its trust store\n    before any call. Tenant verification matches the agent key embedded in the client certificate against\n    the agent key embedded in the trusted CA.\n  validation_point: TLS handshake\ndocs:\n- https://docs.silverflow.com/guides/authentication\n- https://docs.silverflow.com/guides/getting-started\n- https://docs.silverflow.com/apidocs/latest/index.html#tag/API-Keys\nname: Silverflow authentication\nrequired_on: every endpoint and method — \"The Silverflow API requires authentication on all endpoints\n  and methods.\"\ndefault_security:\n- ApiKey: []\n- BearerToken: []\noauth2:\n  supported: false\n  note: No oauth2 or openIdConnect security scheme is declared and no OAuth authorization-server metadata\n    is served at /.well-known/oauth-authorization-server on any host (all 404). No scopes/ artifact was\n    written — there is no scope\
  \ surface to record.\ntoken_prefixes:\n  api_key: apk-\n  agent: cgt-\nsecrets_handling: The API key secret is shown once. Rotation is create-new -> switch -> delete-old, using\n  the 40-key allowance.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silverflow/refs/heads/main/authentication/silverflow-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Payments
- Card Processing
- Acquiring
- Financial Services
- Tokenization
- 3-D Secure
- Disputes
- Chargebacks
- Interchange
- Reconciliation
- Point of Sale
- Netherlands
---
