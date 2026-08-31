---
api_key_in: []
api_specs:
- filename: select-medical-holdings-fhir-r4-openapi.yml
  format: yaml
  label: Select Medical FHIR R4 API
  slug: select-medical-holdings-fhir-r4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/select-medical-holdings/refs/heads/main/openapi/select-medical-holdings-fhir-r4-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Select Medical Holdings Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- jwtBearer
- refreshToken
overview: Select Medical Holdings secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, jwtBearer, and refreshToken flow(s).
provider_name: Select Medical Holdings
provider_slug: select-medical-holdings
scheme_count: 2
schemes:
- description: SMART-on-FHIR OAuth 2.0. The CapabilityStatement advertises the authorize and token URIs via the standard SMART oauth-uris extension, and declares OAuth + SMART-on-FHIR under rest.security.service.
  flows:
  - authorizationUrl: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/authorize
    flow: authorizationCode
    pkce: true
    pkce_methods:
    - S256
    tokenUrl: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/token
  - flow: clientCredentials
    note: Backend-services flow; requires asymmetric (private_key_jwt) client authentication.
    tokenUrl: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/token
  - flow: jwtBearer
    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/token
  name: smartOnFhir
  smart_capabilities:
  - launch-ehr
  - launch-standalone
  - client-public
  - client-confidential-symmetric
  - client-confidential-asymmetric
  - context-banner
  - context-style
  - context-ehr-patient
  - context-ehr-encounter
  - context-standalone-patient
  - permission-offline
  - permission-patient
  - permission-user
  - permission-v1
  - permission-v2
  - sso-openid-connect
  - authorize-post
  sources:
  - https://epicproxy.et0948.epichosted.com/FhirProxy/api/FHIR/R4/.well-known/smart-configuration
  - fhir/select-medical-holdings-r4-capabilitystatement.json
  standard: SMART App Launch (SMART on FHIR)
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: oauth2
- description: OpenID Connect discovery is served at the FhirProxy oauth2 issuer, so the same credentials carry an identity assertion (sso-openid-connect is declared among the SMART capabilities).
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2
  jwks_uri: https://epicproxy.et0948.epichosted.com/FhirProxy/api/epic/2019/Security/Open/PublicKeys/530027/OIDC
  name: openIdConnect
  openIdConnectUrl: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/.well-known/openid-configuration
  sources:
  - https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/.well-known/openid-configuration
  subject_types_supported:
  - public
  type: openIdConnect
slug: select-medical-holdings-authentication
source_filename: select-medical-holdings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: https://epicproxy.et0948.epichosted.com/FhirProxy/api/FHIR/R4/.well-known/smart-configuration\ndocs: https://fhir.epic.com/Documentation?docId=oauth2\nnote: >-\n  Read directly from the two discovery documents the Select Medical FHIR server serves anonymously\n  (smart-configuration HTTP 200, openid-configuration HTTP 200, both fetched 2026-08-28), and\n  cross-checked against the security block of the server's own CapabilityStatement. This is a\n  SMART-on-FHIR deployment on Epic; there is no API-key or basic-auth path.\nsummary:\n  types:\n    - oauth2\n    - openIdConnect\n  oauth2_flows:\n    - authorizationCode\n    - clientCredentials\n    - jwtBearer\n    - refreshToken\n  public_registration: false\n  registration_note: >-\n    App registration is not self-serve at Select Medical. Client IDs are issued through Epic's\n    App Orchard / Vendor Services program and then activated by the health system, so an agent\n    cannot\
  \ obtain credentials from the endpoint alone.\nschemes:\n  - name: smartOnFhir\n    type: oauth2\n    standard: SMART App Launch (SMART on FHIR)\n    description: >-\n      SMART-on-FHIR OAuth 2.0. The CapabilityStatement advertises the authorize and token URIs via the\n      standard SMART oauth-uris extension, and declares OAuth + SMART-on-FHIR under rest.security.service.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/authorize\n        tokenUrl: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/token\n        pkce: true\n        pkce_methods:\n          - S256\n      - flow: clientCredentials\n        tokenUrl: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/token\n        note: Backend-services flow; requires asymmetric (private_key_jwt) client authentication.\n      - flow: jwtBearer\n        grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer\n        tokenUrl: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/token\n\
  \    token_endpoint_auth_methods:\n      - client_secret_post\n      - client_secret_basic\n      - private_key_jwt\n    smart_capabilities:\n      - launch-ehr\n      - launch-standalone\n      - client-public\n      - client-confidential-symmetric\n      - client-confidential-asymmetric\n      - context-banner\n      - context-style\n      - context-ehr-patient\n      - context-ehr-encounter\n      - context-standalone-patient\n      - permission-offline\n      - permission-patient\n      - permission-user\n      - permission-v1\n      - permission-v2\n      - sso-openid-connect\n      - authorize-post\n    sources:\n      - https://epicproxy.et0948.epichosted.com/FhirProxy/api/FHIR/R4/.well-known/smart-configuration\n      - fhir/select-medical-holdings-r4-capabilitystatement.json\n  - name: openIdConnect\n    type: openIdConnect\n    description: >-\n      OpenID Connect discovery is served at the FhirProxy oauth2 issuer, so the same credentials carry\n      an identity assertion (sso-openid-connect\
  \ is declared among the SMART capabilities).\n    issuer: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2\n    openIdConnectUrl: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/.well-known/openid-configuration\n    jwks_uri: https://epicproxy.et0948.epichosted.com/FhirProxy/api/epic/2019/Security/Open/PublicKeys/530027/OIDC\n    id_token_signing_alg_values_supported:\n      - RS256\n    subject_types_supported:\n      - public\n    sources:\n      - https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/.well-known/openid-configuration\nx-evidence:\n  - url: https://epicproxy.et0948.epichosted.com/FhirProxy/api/FHIR/R4/.well-known/smart-configuration\n    http_status: 200\n    content_type: application/json; charset=utf-8\n    fetched: '2026-08-28'\n  - url: https://epicproxy.et0948.epichosted.com/FhirProxy/oauth2/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json; charset=utf-8\n    fetched: '2026-08-28'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/select-medical-holdings/refs/heads/main/authentication/select-medical-holdings-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Healthcare
- Hospitals
- Rehabilitation
- Patient Access
- FHIR
- Interoperability
- Electronic Health Records
- Fortune 1000
---
