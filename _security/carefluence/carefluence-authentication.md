---
api_key_in: []
api_specs:
- filename: postman.yaml
  format: yaml
  label: Carefluence Open API R4
  slug: openapi-r4
  spec_type: Postman
  url: https://api.carefluence.com/
auth_types: []
description: Carefluence Open API R4 is a SMART-on-FHIR surface. Every resource call carries an OAuth 2.0 bearer token in the Authorization header; tokens are issued by a first-party IdentityServer-style OpenID Connect authorization server at https://core.carefluence.com/cf.admin.core. There is no API-key path.
kind: authentication
layout: security
method: probed
name: Carefluence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carefluence declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Carefluence
provider_slug: carefluence
scheme_count: 2
schemes:
- description: OAuth 2.0 + OpenID Connect, profiled by SMART App Launch. The provider's own documentation states the authorization code grant is the only grant it recommends for app developers ("the only grant type supported in this release because it is considered secure"), although the discovery document advertises a wider set.
  endpoints:
    authorization: https://core.carefluence.com/cf.admin.core/connect/authorize
    check_session_iframe: https://core.carefluence.com/cf.admin.core/connect/checksession
    device_authorization: https://core.carefluence.com/cf.admin.core/connect/deviceauthorization
    end_session: https://core.carefluence.com/cf.admin.core/connect/endsession
    introspection: https://core.carefluence.com/cf.admin.core/connect/introspect
    jwks: https://core.carefluence.com/cf.admin.core/.well-known/openid-configuration/jwks
    revocation: https://core.carefluence.com/cf.admin.core/connect/revocation
    token: https://core.carefluence.com/cf.admin.core/connect/token
    userinfo: https://core.carefluence.com/cf.admin.core/connect/userinfo
  format: Bearer <access_token>
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  header: Authorization
  id: smart_on_fhir_oauth2
  id_token_signing_alg_values:
  - RS256
  in: header
  issuer: https://core.carefluence.com/cf.admin.core
  pkce:
    code_challenge_methods:
    - plain
    - S256
    supported: true
  response_modes_supported:
  - form_post
  - query
  - fragment
  response_types_supported:
  - code
  - token
  - id_token
  - id_token token
  - code id_token
  - code token
  - code id_token token
  scopes_documented: scopes/carefluence-scopes.yml
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  type: oauth2
- claims_supported:
  - address
  - email
  - email_verified
  - sub
  - phone
  - phone_verified
  - name
  - family_name
  - given_name
  - middle_name
  - nickname
  - preferred_username
  - profile
  - picture
  - website
  - gender
  - birthdate
  - zoneinfo
  - locale
  - updated_at
  description: Full OpenID Connect discovery is served anonymously; front-channel and back-channel logout are both advertised as supported.
  id: openid_connect
  openIdConnectUrl: https://core.carefluence.com/cf.admin.core/.well-known/openid-configuration
  type: openIdConnect
slug: carefluence-authentication
source_filename: carefluence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  https://core.carefluence.com/cf.admin.core/.well-known/openid-configuration\n  (HTTP 200), https://classic.carefluence.com/r4/.well-known/smart-configuration\n  (HTTP 200), the CapabilityStatement security block at\n  https://classic.carefluence.com/r4/metadata (HTTP 200), and the\n  \"Security & Authorization Flow\" section of the published Postman collection\n  at https://api.carefluence.com/\nname: Carefluence Open API R4 authentication\ndescription: >-\n  Carefluence Open API R4 is a SMART-on-FHIR surface. Every resource call\n  carries an OAuth 2.0 bearer token in the Authorization header; tokens are\n  issued by a first-party IdentityServer-style OpenID Connect authorization\n  server at https://core.carefluence.com/cf.admin.core. There is no API-key\n  path.\nschemes:\n- id: smart_on_fhir_oauth2\n  type: oauth2\n  in: header\n  header: Authorization\n  format: 'Bearer <access_token>'\n  description: >-\n    OAuth\
  \ 2.0 + OpenID Connect, profiled by SMART App Launch. The provider's\n    own documentation states the authorization code grant is the only grant it\n    recommends for app developers (\"the only grant type supported in this\n    release because it is considered secure\"), although the discovery document\n    advertises a wider set.\n  issuer: https://core.carefluence.com/cf.admin.core\n  endpoints:\n    authorization: https://core.carefluence.com/cf.admin.core/connect/authorize\n    token: https://core.carefluence.com/cf.admin.core/connect/token\n    userinfo: https://core.carefluence.com/cf.admin.core/connect/userinfo\n    introspection: https://core.carefluence.com/cf.admin.core/connect/introspect\n    revocation: https://core.carefluence.com/cf.admin.core/connect/revocation\n    end_session: https://core.carefluence.com/cf.admin.core/connect/endsession\n    check_session_iframe: https://core.carefluence.com/cf.admin.core/connect/checksession\n    device_authorization: https://core.carefluence.com/cf.admin.core/connect/deviceauthorization\n\
  \    jwks: https://core.carefluence.com/cf.admin.core/.well-known/openid-configuration/jwks\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - 'urn:ietf:params:oauth:grant-type:device_code'\n  response_types_supported: [code, token, id_token, 'id_token token', 'code id_token', 'code token', 'code id_token token']\n  response_modes_supported: [form_post, query, fragment]\n  pkce:\n    supported: true\n    code_challenge_methods: [plain, S256]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt]\n  id_token_signing_alg_values: [RS256]\n  subject_types: [public]\n  scopes_documented: scopes/carefluence-scopes.yml\n- id: openid_connect\n  type: openIdConnect\n  openIdConnectUrl: https://core.carefluence.com/cf.admin.core/.well-known/openid-configuration\n  description: >-\n    Full OpenID Connect discovery is served anonymously; front-channel and\n    back-channel logout are both\
  \ advertised as supported.\n  claims_supported: [address, email, email_verified, sub, phone, phone_verified, name, family_name,\n    given_name, middle_name, nickname, preferred_username, profile, picture, website, gender,\n    birthdate, zoneinfo, locale, updated_at]\nsmart_on_fhir:\n  discovery: https://classic.carefluence.com/r4/.well-known/smart-configuration\n  capabilities:\n  - launch-ehr\n  - launch-standalone\n  - client-public\n  - client-confidential-symmetric\n  - sso-openid-connect\n  - context-banner\n  - context-style\n  - context-ehr-patient\n  - context-standalone-patient\n  - context-standalone-encounter\n  - permission-offline\n  - permission-patient\n  - permission-user\n  client_types:\n  - id: confidential\n    description: Clients that can protect a client_secret (server-side web apps, native mobile clients per the provider's docs).\n  - id: public\n    description: Clients that cannot protect a secret; supported via PKCE and the public client registration path.\n\
  \  capability_statement_security:\n    service: SMART-on-FHIR\n    system: http://terminology.hl7.org/CodeSystem/restful-security-service\n    oauth_uris_extension: http://fhir-registry.smarthealthit.org/StructureDefinition/oauth-uris\nonboarding:\n  developer_registration: https://core.carefluence.com/cf.admin.core/Account/RegisterDeveloper\n  developer_login: https://core.carefluence.com/cf.admin.core/Account/Login\n  approval_required: true\n  approval_note: >-\n    Registered developers register an application and the grants must be\n    approved by Carefluence administration before tokens are issued. Stated\n    verbatim in the Postman collection's Client Registration section.\nmulti_factor_authentication:\n  available: true\n  optional_add_on: true\n  module: Carefluence SMART Connect\n  applies_to: [api-administrators, self-registered-developers, patients]\n  delivery: [email, sms]\n  note: >-\n    The provider states SMART Connect MFA is an option when the Open API\n    platform\
  \ is deployed in Microsoft Azure, and that the platform can also\n    work with a customer's other MFA provider.\n  source: https://api.carefluence.com/ (\"Multi-factor Authentication Option\" section)\ntoken_response_shape:\n  access_token: string\n  token_type: Bearer\n  expires_in: 1200\n  note: Example lifetime published in the provider's own authorization walkthrough (1200 seconds).\ngaps:\n- No API-key or mutual-TLS path is documented for this API.\n- >-\n  The provider's prose says authorization_code is the only supported grant,\n  while the live discovery document advertises implicit, password and\n  client_credentials as well. Treat the discovery document as the machine\n  truth and the prose as the supported-integration guidance.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carefluence/refs/heads/main/authentication/carefluence-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Healthcare
- Interoperability
- FHIR
- HL7
- SMART on FHIR
- Electronic Health Records
- Clinical Data
- Health IT
- ONC Certified
- USCDI
- OAuth 2.0
- Telehealth
- Health Information Exchange
---
