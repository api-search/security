---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ss-c-technologies-marketdataservice-api-openapi.yml
  format: yaml
  label: SS&C Technologies Market Data Service API
  slug: ss-c-technologies-marketdataservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-marketdataservice-api-openapi.yml
- filename: ss-c-technologies-submitorderservice-api-openapi.yml
  format: yaml
  label: SS&C Technologies Submit Order Service API
  slug: ss-c-technologies-submitorderservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-submitorderservice-api-openapi.yml
- filename: ss-c-technologies-userservices-api-openapi.yml
  format: yaml
  label: SS&C Technologies User Services API
  slug: ss-c-technologies-userservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-userservices-api-openapi.yml
- filename: ss-c-technologies-xapiserver-api-openapi.yml
  format: yaml
  label: SS&C Technologies XAPI Server API
  slug: ss-c-technologies-xapiserver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-xapiserver-api-openapi.yml
- filename: ss-c-technologies-utility-services-api-openapi.yml
  format: yaml
  label: SS&C Technologies Utility Services API
  slug: ss-c-technologies-utility-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-utility-services-api-openapi.yml
auth_types:
- http
- session-token
- srp
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Ss C Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: SS&C Technologies secures its APIs with http, session-token, srp, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SS&C Technologies
provider_slug: ss-c-technologies
scheme_count: 5
schemes:
- applies_to: SS&C Eze EMS xAPI REST surface
  bearerFormat: JWT
  description: 'Please enter a valid token :'
  name: Bearer
  note: 'The only securityScheme the OpenAPI declares, and it is applied globally via a root-level `security: [{Bearer: []}]`. The spec gives no token-issuance endpoint for this bearer token and no description beyond the placeholder text above.'
  scheme: Bearer
  sources:
  - openapi/ss-c-technologies-eze-ems-xapi-openapi.json
  type: http
- applies_to: both the gRPC and REST surfaces
  description: The working credential for Eze EMS xAPI. UtilityServices.Connect (REST GET /api/v1/authentication/connect) takes UserName, Domain, Password and Locale and returns a UserToken in ConnectResponse; SS&C's own tutorial states the token "must be provided on all subsequent calls to the server". UtilityServices.Disconnect ends the session.
  in: query
  name: UserToken
  note: On the REST projection the login parameters and the UserToken are carried as QUERY parameters, including Password on GET /api/v1/authentication/connect and GET /api/v1/authentication/change-password. This is recorded because it is what the published contract says, not as an assessment.
  parameter: UserToken
  sources:
  - grpc/ss-c-technologies-xapi-utilities.proto
  - openapi/ss-c-technologies-eze-ems-xapi-openapi.json
  type: session-token
- applies_to: SS&C Eze EMS xAPI, where the client domain is SRP-enabled
  availability: SS&C's FAQ states both SRP and standard login work on an SRP-enabled domain, and only standard login works on a domain that is not SRP-enabled. Whether a domain is SRP-enabled is set by SS&C.
  description: Secure Remote Password (SRP) login, a zero-knowledge password proof, exposed as the StartLoginSrp / CompleteLoginSrp RPC pair (REST GET /api/v1/authentication/start-login-srp and /api/v1/authentication/complete-login-srp) plus ChangePasswordSRP.
  name: SRP
  sources:
  - grpc/ss-c-technologies-xapi-utilities.proto
  - https://github.com/ezesoft/xapi/blob/master/faq.md
  type: srp
- applies_to: SS&C Eze EMS xAPI
  description: UtilityServices.MultiFactorAuthentication (REST GET /api/v1/authentication/multi-factor-authentication). ConnectResponse carries MFASecurityCode, MFAtotpPreference and MFAtotpValue fields, so TOTP is a supported second factor.
  name: MFA
  sources:
  - grpc/ss-c-technologies-xapi-utilities.proto
  type: mfa
- applies_to: the SS&C APIM developer portal (developer.ssctech.com / apim.ssnc.cloud)
  description: A Keycloak realm named APIM. The discovery document advertises authorization_code, client_credentials, implicit, password, refresh_token, device_code, jwt-bearer, token-exchange, uma-ticket and CIBA grants, PKCE (S256), and a scope list that includes one API-specific scope, events_enrichment_api_member.
  name: SS&C APIM OpenID Connect
  note: This governs the developer portal and the Kong gateway it fronts, not the Eze EMS xAPI. Every portal catalog endpoint probed anonymously 302s to https://developer.ssctech.com/sso/login.
  openIdConnectUrl: https://ssoprod.ssnc.cloud/auth/realms/APIM/.well-known/openid-configuration
  sources:
  - well-known/ss-c-technologies-openid-configuration.json
  type: openIdConnect
slug: ss-c-technologies-authentication
source_filename: ss-c-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: >-\n  openapi/ss-c-technologies-eze-ems-xapi-openapi.json,\n  grpc/ss-c-technologies-xapi-utilities.proto,\n  https://github.com/ezesoft/xapi/blob/master/readme.md,\n  https://github.com/ezesoft/xapi/blob/master/faq.md,\n  https://ssoprod.ssnc.cloud/auth/realms/APIM/.well-known/openid-configuration\ndocs: https://github.com/ezesoft/xapi/blob/master/readme.md#tutorial-1-connecting-and-disconnecting\nsummary:\n  types:\n  - http\n  - session-token\n  - srp\n  - openIdConnect\nschemes:\n- name: Bearer\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  description: 'Please enter a valid token :'\n  applies_to: SS&C Eze EMS xAPI REST surface\n  sources:\n  - openapi/ss-c-technologies-eze-ems-xapi-openapi.json\n  note: >-\n    The only securityScheme the OpenAPI declares, and it is applied globally via a root-level\n    `security: [{Bearer: []}]`. The spec gives no token-issuance endpoint for this bearer token and\n    no description\
  \ beyond the placeholder text above.\n- name: UserToken\n  type: session-token\n  in: query\n  parameter: UserToken\n  applies_to: both the gRPC and REST surfaces\n  sources:\n  - grpc/ss-c-technologies-xapi-utilities.proto\n  - openapi/ss-c-technologies-eze-ems-xapi-openapi.json\n  description: >-\n    The working credential for Eze EMS xAPI. UtilityServices.Connect (REST GET\n    /api/v1/authentication/connect) takes UserName, Domain, Password and Locale and returns a\n    UserToken in ConnectResponse; SS&C's own tutorial states the token \"must be provided on all\n    subsequent calls to the server\". UtilityServices.Disconnect ends the session.\n  note: >-\n    On the REST projection the login parameters and the UserToken are carried as QUERY parameters,\n    including Password on GET /api/v1/authentication/connect and\n    GET /api/v1/authentication/change-password. This is recorded because it is what the published\n    contract says, not as an assessment.\n- name: SRP\n  type: srp\n\
  \  applies_to: SS&C Eze EMS xAPI, where the client domain is SRP-enabled\n  sources:\n  - grpc/ss-c-technologies-xapi-utilities.proto\n  - https://github.com/ezesoft/xapi/blob/master/faq.md\n  description: >-\n    Secure Remote Password (SRP) login, a zero-knowledge password proof, exposed as the\n    StartLoginSrp / CompleteLoginSrp RPC pair (REST GET /api/v1/authentication/start-login-srp and\n    /api/v1/authentication/complete-login-srp) plus ChangePasswordSRP.\n  availability: >-\n    SS&C's FAQ states both SRP and standard login work on an SRP-enabled domain, and only standard\n    login works on a domain that is not SRP-enabled. Whether a domain is SRP-enabled is set by SS&C.\n- name: MFA\n  type: mfa\n  applies_to: SS&C Eze EMS xAPI\n  sources:\n  - grpc/ss-c-technologies-xapi-utilities.proto\n  description: >-\n    UtilityServices.MultiFactorAuthentication (REST GET\n    /api/v1/authentication/multi-factor-authentication). ConnectResponse carries MFASecurityCode,\n    MFAtotpPreference\
  \ and MFAtotpValue fields, so TOTP is a supported second factor.\n- name: SS&C APIM OpenID Connect\n  type: openIdConnect\n  openIdConnectUrl: https://ssoprod.ssnc.cloud/auth/realms/APIM/.well-known/openid-configuration\n  applies_to: the SS&C APIM developer portal (developer.ssctech.com / apim.ssnc.cloud)\n  sources:\n  - well-known/ss-c-technologies-openid-configuration.json\n  description: >-\n    A Keycloak realm named APIM. The discovery document advertises authorization_code,\n    client_credentials, implicit, password, refresh_token, device_code, jwt-bearer, token-exchange,\n    uma-ticket and CIBA grants, PKCE (S256), and a scope list that includes one API-specific scope,\n    events_enrichment_api_member.\n  note: >-\n    This governs the developer portal and the Kong gateway it fronts, not the Eze EMS xAPI. Every\n    portal catalog endpoint probed anonymously 302s to https://developer.ssctech.com/sso/login.\ncredential_acquisition:\n  self_serve: false\n  note: >-\n    No surface\
  \ here issues credentials without a human. SS&C Eze says \"Server details and\n    authentication credentials will be provided by your SS&C Eze representative\"; the SS&C APIM\n    portal says to contact a Client Relationship manager; Black Diamond routes new partners to a\n    request form and existing clients to their account team.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/authentication/ss-c-technologies-authentication.yml
summary_line: http/session-token/srp/openIdConnect · 5 schemes
tags:
- Financial Services
- Investment Management
- Fund Administration
- Wealth Management
- Execution Management
- Order Management
- Market Data
- Trading
- gRPC
- Enterprise Software
---
