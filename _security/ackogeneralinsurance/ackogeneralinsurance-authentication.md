---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ackogeneralinsurance-enterprise-openapi.yml
  format: yaml
  label: ACKO for Enterprise Partnership API
  slug: acko-for-enterprise-partnership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ackogeneralinsurance/refs/heads/main/openapi/ackogeneralinsurance-enterprise-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ackogeneralinsurance Authentication
name_suffix: Authentication
oauth_flows: []
overview: ACKO General Insurance declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ACKO General Insurance
provider_slug: ackogeneralinsurance
scheme_count: 2
schemes:
- evidence: openapi/_original/ackogeneralinsurance-enterprise-openapi.json#/paths/~1realms~1partnership~1protocol~1openid-connect~1token/post
  flow: clientCredentials
  id: partnership-oauth2-client-credentials
  parameters:
  - description: Type of grant being requested
    in: query
    name: grant_type
    required: true
  - description: The unique identifier for the partner
    in: query
    name: client_id
    required: true
  - description: The secret key associated with the partner's client_id
    in: query
    name: client_secret
    required: true
  response_fields:
  - accessToken
  - expiresIn
  - refreshExpiresIn
  - tokenType
  - notBeforePolicy
  - scope
  scopes_enumerated: false
  scopes_note: The token response carries a `scope` string but the documentation enumerates no scope values, so no scopes/ artifact is derivable. Requesting an OAuth scope reference is a provider follow-up.
  token_url: https://www.acko.com/realms/partnership/protocol/openid-connect/token
  type: oauth2
- description_verbatim: '"username={partner} algorithm={algo} created_on={time} secret={secret}   This will be shared over mail when the product is onboarded"'
  evidence: https://www.acko.com/external/partnership/policy
  id: partnership-authorization-header
  in: header
  name: Authorization
  note: On the token endpoint the Authorization header carries the partner signature string quoted above. On the 29 business operations the header is documented only as a required Authorization header; the live gateway rejects a non-bearer value with 401 "Not a bearer token", so business calls carry the OAuth 2.0 bearer access token from tokenGeneration.
  required_on_operations: 30
  type: http
slug: ackogeneralinsurance-authentication
source_filename: ackogeneralinsurance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://www.acko.com/enterprise/documentation/enterprise.html\nspec_source: openapi/_original/ackogeneralinsurance-enterprise-openapi.json\nnote: >-\n  The published OpenAPI declares NO components.securitySchemes. The auth model below is read from the\n  Authentication tag description, the tokenGeneration operation, and the Authorization header\n  parameter that every one of the 30 operations marks required. Confirmed live: an unauthenticated\n  GET https://www.acko.com/external/partnership/policy returns 401\n  {\"error\":\"Invalid token, error: Not a bearer token\"}.\nsummary:\n  primary_model: oauth2-client-credentials\n  token_endpoint: https://www.acko.com/realms/partnership/protocol/openid-connect/token\n  token_endpoint_operation_id: tokenGeneration\n  identity_provider: Keycloak (realm \"partnership\", RESTEasy OIDC token endpoint observed live)\n  scheme_count_declared_in_spec: 0\n  operations_requiring_auth: 30\n\
  \  onboarding: >-\n    Client credentials are issued by ACKO when a partner product is onboarded; the spec states the\n    credential material \"will be shared over mail when the product is onboarded\". There is no\n    self-serve signup for the partnership API.\nschemes:\n- id: partnership-oauth2-client-credentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://www.acko.com/realms/partnership/protocol/openid-connect/token\n  parameters:\n  - name: grant_type\n    in: query\n    required: true\n    description: Type of grant being requested\n  - name: client_id\n    in: query\n    required: true\n    description: The unique identifier for the partner\n  - name: client_secret\n    in: query\n    required: true\n    description: The secret key associated with the partner's client_id\n  response_fields:\n  - accessToken\n  - expiresIn\n  - refreshExpiresIn\n  - tokenType\n  - notBeforePolicy\n  - scope\n  scopes_enumerated: false\n  scopes_note: >-\n    The token response\
  \ carries a `scope` string but the documentation enumerates no scope values, so\n    no scopes/ artifact is derivable. Requesting an OAuth scope reference is a provider follow-up.\n  evidence: openapi/_original/ackogeneralinsurance-enterprise-openapi.json#/paths/~1realms~1partnership~1protocol~1openid-connect~1token/post\n- id: partnership-authorization-header\n  type: http\n  in: header\n  name: Authorization\n  required_on_operations: 30\n  description_verbatim: >-\n    \"username={partner} algorithm={algo} created_on={time} secret={secret}   This will be shared over\n    mail when the product is onboarded\"\n  note: >-\n    On the token endpoint the Authorization header carries the partner signature string quoted above.\n    On the 29 business operations the header is documented only as a required Authorization header;\n    the live gateway rejects a non-bearer value with 401 \"Not a bearer token\", so business calls\n    carry the OAuth 2.0 bearer access token from tokenGeneration.\n\
  \  evidence: https://www.acko.com/external/partnership/policy\nerrors:\n- status: 401\n  schema: InvalidClientCredentials\n  example:\n    error: unauthorized_client\n    error_description: Invalid client or Invalid client credentials\ngaps:\n- securitySchemes are absent from the published OpenAPI, so no machine-readable auth binding exists.\n- No scope reference is published.\n- No token TTL / refresh policy is documented beyond the expiresIn and refreshExpiresIn response fields.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ackogeneralinsurance/refs/heads/main/authentication/ackogeneralinsurance-authentication.yml
summary_line: 2 schemes
tags:
- Insurance
- Insurtech
- Embedded Insurance
- Health Insurance
- Travel Insurance
- Claims
- Policy Administration
- Financial Services
- India
- Enterprise
---
