---
api_key_in: []
api_specs:
- filename: athelas-enterprise-openapi.yml
  format: yaml
  label: Athelas Enterprise API
  slug: athelas-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athelas/refs/heads/main/openapi/athelas-enterprise-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Athelas Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Athelas secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Athelas
provider_slug: athelas
scheme_count: 2
schemes:
- api: Athelas Enterprise API
  description: 'Bearer token for the Athelas Enterprise RPM API. Obtain a token by POSTing email and password to /auth/login (production https://api.athelas.com/enterprise/v1, staging https://staging-api.athelas.com/enterprise/v1). Tokens expire after 60 minutes and must be renewed by repeating the login. Sent as Authorization: Bearer <token>.'
  docs: https://athelas.readme.io/docs/authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/athelas-enterprise-openapi.yml
  type: http
- api: Commure EHR FHIR API
  description: 'SMART on FHIR v2 (ONC §170.215(a)(3)) using AWS Cognito as the identity provider. Access tokens are sent as Authorization: Bearer <token> on all FHIR requests. Supports standalone launch, EHR launch, and Backend Services (bulk data) authorization. Token endpoint auth methods: none (PKCE), client_secret_post, client_secret_basic, private_key_jwt. PKCE S256 required for public clients. Refresh tokens issued only with offline_access scope; confidential-client tokens valid a minimum of 3 months.'
  docs: https://docs.athelas.com/air_developer/fhir_api/commure_ehr_fhir_api
  flows:
  - authorizationUrl: https://onc.api.staging-ehr.athelas.com/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://onc.api.staging-ehr.athelas.com/token
  - client_assertion: private_key_jwt
    flow: clientCredentials
    note: Backend Services Authorization (bulk data / system-level)
    tokenUrl: https://onc.api.staging-ehr.athelas.com/token
  - flow: refreshToken
    tokenUrl: https://onc.api.staging-ehr.athelas.com/token
  introspection_endpoint: https://onc.api.staging-ehr.athelas.com/introspect
  issuer: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_KudjXF579
  jwks_uri: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_KudjXF579/.well-known/jwks.json
  name: smartOnFhir
  revocation_endpoint: https://onc.api.staging-ehr.athelas.com/revoke
  scopes_ref: scopes/athelas-scopes.yml
  type: oauth2
  well_known: https://onc.api.staging-ehr.athelas.com/.well-known/smart-configuration
slug: athelas-authentication
source_filename: athelas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/athelas-enterprise-openapi.yml\ndocs:\n- https://athelas.readme.io/docs/authentication\n- https://docs.athelas.com/air_developer/fhir_api/commure_ehr_fhir_api\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\nschemes:\n- name: bearerAuth\n  api: Athelas Enterprise API\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token for the Athelas Enterprise RPM API. Obtain a token by POSTing email\n    and password to /auth/login (production https://api.athelas.com/enterprise/v1,\n    staging https://staging-api.athelas.com/enterprise/v1). Tokens expire after 60\n    minutes and must be renewed by repeating the login. Sent as\n    Authorization: Bearer <token>.\n  sources:\n  - openapi/athelas-enterprise-openapi.yml\n  docs: https://athelas.readme.io/docs/authentication\n- name: smartOnFhir\n  api: Commure EHR FHIR API\n  type: oauth2\n \
  \ description: >-\n    SMART on FHIR v2 (ONC §170.215(a)(3)) using AWS Cognito as the identity provider.\n    Access tokens are sent as Authorization: Bearer <token> on all FHIR requests.\n    Supports standalone launch, EHR launch, and Backend Services (bulk data)\n    authorization. Token endpoint auth methods: none (PKCE), client_secret_post,\n    client_secret_basic, private_key_jwt. PKCE S256 required for public clients.\n    Refresh tokens issued only with offline_access scope; confidential-client tokens\n    valid a minimum of 3 months.\n  issuer: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_KudjXF579\n  jwks_uri: https://cognito-idp.us-east-2.amazonaws.com/us-east-2_KudjXF579/.well-known/jwks.json\n  well_known: https://onc.api.staging-ehr.athelas.com/.well-known/smart-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://onc.api.staging-ehr.athelas.com/authorize\n    tokenUrl: https://onc.api.staging-ehr.athelas.com/token\n    pkce: S256\n\
  \  - flow: clientCredentials\n    tokenUrl: https://onc.api.staging-ehr.athelas.com/token\n    client_assertion: private_key_jwt\n    note: Backend Services Authorization (bulk data / system-level)\n  - flow: refreshToken\n    tokenUrl: https://onc.api.staging-ehr.athelas.com/token\n  introspection_endpoint: https://onc.api.staging-ehr.athelas.com/introspect\n  revocation_endpoint: https://onc.api.staging-ehr.athelas.com/revoke\n  scopes_ref: scopes/athelas-scopes.yml\n  docs: https://docs.athelas.com/air_developer/fhir_api/commure_ehr_fhir_api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athelas/refs/heads/main/authentication/athelas-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Healthcare
- Remote Patient Monitoring
- Electronic Health Records
- FHIR
- Revenue Cycle Management
- Medical Devices
- SMART on FHIR
- Interoperability
- AI
---
