---
anonymous_access: false
api_key_in: []
api_specs:
- filename: guidewire-integration-gateway-asyncapi.yml
  format: yaml
  label: Guidewire Integration Gateway API
  slug: guidewire-integration-gateway-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/asyncapi/guidewire-integration-gateway-asyncapi.yml
- filename: guidewire-accounts-api-openapi.yml
  format: yaml
  label: Guidewire Accounts API
  slug: guidewire-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-accounts-api-openapi.yml
- filename: guidewire-claims-api-openapi.yml
  format: yaml
  label: Guidewire Claims API
  slug: guidewire-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-claims-api-openapi.yml
- filename: guidewire-exposures-api-openapi.yml
  format: yaml
  label: Guidewire Exposures API
  slug: guidewire-exposures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-exposures-api-openapi.yml
- filename: guidewire-fnol-api-openapi.yml
  format: yaml
  label: Guidewire FNOL API
  slug: guidewire-fnol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-fnol-api-openapi.yml
- filename: guidewire-payments-api-openapi.yml
  format: yaml
  label: Guidewire Payments API
  slug: guidewire-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-payments-api-openapi.yml
- filename: guidewire-policies-api-openapi.yml
  format: yaml
  label: Guidewire Policies API
  slug: guidewire-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-policies-api-openapi.yml
- filename: guidewire-quotes-api-openapi.yml
  format: yaml
  label: Guidewire Quotes API
  slug: guidewire-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-quotes-api-openapi.yml
auth_types:
- http-basic
- bearer-jwt
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Guidewire Authentication
name_suffix: Authentication
oauth_flows: []
overview: Guidewire secures its APIs with http-basic and bearer-jwt across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Guidewire
provider_slug: guidewire
scheme_count: 2
schemes:
- applies_to:
  - internal user
  - external user
  - anonymous user
  - standalone service
  - service-for-user
  - service-for-service
  bearer_format: JWT
  construct_jwt_docs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthChoose/overview-authentication/c_constructing_jwts.html
  description: The caller presents a JSON Web Token. The JWT carries BOTH authentication and authorization information as token claims. This is the only method supported in production.
  docs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthChoose/overview-authentication/c_authentication-methods.html
  name: BearerJWT
  scheme: bearer
  token_issuer: The customer's identity provider, configured per Guidewire Cloud deployment. Guidewire does not operate a public authorization server for Cloud API and publishes no authorization_endpoint, token_endpoint, JWKS URI or grant-type list.
  type: http
- applies_to:
  - internal user
  constraint: '"Basic authentication is not supported in production environments. It can only be used in development environments." Quoted verbatim.'
  description: User name and password in the request header; authentication and authorization are read from the operational database.
  docs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthFlows/basic-auth/c_basic-authentication.html
  name: HTTPBasic
  production_supported: false
  scheme: basic
  type: http
slug: guidewire-authentication
source_filename: guidewire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: >-\n  Guidewire InsuranceSuite Cloud API Configuration & Authentication Guide, read from\n  docs.guidewire.com (public, no credentials).\ndocs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthChoose/p_choosing-an-authentication-flow.html\nprovider: guidewire\nproviderId: guidewire\napi: InsuranceSuite Cloud API\nsupersedes: >-\n  A derived profile written from openapi/*.yml on 2026-09-12 that reported an OAuth 2.0\n  authorizationCode flow at https://login.guidewire.com/oauth/authorize and /oauth/token. That host\n  does NOT RESOLVE (NXDOMAIN, checked 2026-09-12) and appears nowhere in Guidewire's documentation.\n  The value came from the documentation-shaped scaffold specs in openapi/, not from Guidewire. This\n  file replaces it with what Guidewire actually publishes.\nsummary:\n  types: [http-basic, bearer-jwt]\n  oauth2_authorization_server: null\n  scope_catalog: false\n  authorization_model: named API\
  \ roles (role.yaml), resource access, proxy-user access\nschemes:\n  - name: BearerJWT\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    applies_to: [internal user, external user, anonymous user, standalone service, service-for-user, service-for-service]\n    description: >-\n      The caller presents a JSON Web Token. The JWT carries BOTH authentication and authorization\n      information as token claims. This is the only method supported in production.\n    token_issuer: >-\n      The customer's identity provider, configured per Guidewire Cloud deployment. Guidewire does not\n      operate a public authorization server for Cloud API and publishes no authorization_endpoint,\n      token_endpoint, JWKS URI or grant-type list.\n    docs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthChoose/overview-authentication/c_authentication-methods.html\n    construct_jwt_docs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthChoose/overview-authentication/c_constructing_jwts.html\n\
  \  - name: HTTPBasic\n    type: http\n    scheme: basic\n    applies_to: [internal user]\n    description: >-\n      User name and password in the request header; authentication and authorization are read from the\n      operational database.\n    production_supported: false\n    constraint: >-\n      \"Basic authentication is not supported in production environments. It can only be used in\n      development environments.\" Quoted verbatim.\n    docs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthFlows/basic-auth/c_basic-authentication.html\ncaller_types:\n  types:\n  - internal user\n  - external user\n  - anonymous user\n  - standalone service\n  - service with user context (GW-User-Context header)\n  - service with service-account mapping\n  docs_note: Each caller type has its own documented authentication flow.\n  docs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthChoose/overview-authentication/c_types-of-callers.html\nauthorization:\n  model:\
  \ API roles\n  description: >-\n    Access is granted through named API roles defined in role.yaml files and assigned to callers. A\n    role names the endpoints it opens, the operations allowed on them, and the fields readable or\n    writable. Three orthogonal access types apply: endpoint access (all callers), resource access\n    (users only, in the base configuration) and proxy-user access (external users and services only).\n  reserved_roles: true\n  docs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthImplement/endpoint-access/c_API-role-files.html\n  access_types_docs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthChoose/overview-authentication/c_types_of_access.html\nfailure_handling:\n  docs: https://docs.guidewire.com/cloud/is/202607/cloudapica/cloudAPI/AuthChoose/overview-authentication/c_authentication-failure-error-messages.html\nunauthenticated_surface:\n  endpoints:\n  - path: <applicationURL>/rest/<APIpath>/openapi.json\n    note:\
  \ >-\n      \"In the base configuration, the API definition endpoints are available to any caller, including\n      unauthenticated\" callers. Deployments may restrict this.\n    docs: https://docs.guidewire.com/cloud/cc/202511/cloudapibf/cloudAPI/topics/101-Fund/01-overview-of-Cloud-API/c_viewing-API-definitions.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/authentication/guidewire-authentication.yml
summary_line: http-basic/bearer-jwt · 2 schemes
tags:
- Insurance
- Policy
- Claims
- Billing
- P&C
---
