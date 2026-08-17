---
api_key_in: []
api_specs:
- filename: medplum-fhir-api-openapi.yml
  format: yaml
  label: Medplum Fhir API
  slug: medplum-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medplum/refs/heads/main/openapi/medplum-fhir-api-openapi.yml
auth_types:
- http
- openIdConnect
- oauth2 (SMART App Launch 2.0.0, not declared in OpenAPI securitySchemes)
description: ''
kind: authentication
layout: security
method: searched
name: Medplum Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Medplum secures its APIs with http, openIdConnect, and oauth2 (SMART App Launch 2.0.0, not declared in OpenAPI securitySchemes) across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Medplum
provider_slug: medplum
scheme_count: 4
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/medplum-fhir-api-openapi.yml
  type: http
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/medplum-fhir-api-openapi.yml
  type: http
- name: OpenID
  openIdConnectUrl: https://api.medplum.com/.well-known/openid-configuration
  sources:
  - openapi/medplum-fhir-api-openapi.yml
  type: openIdConnect
- authorizationUrl: https://api.medplum.com/oauth2/authorize
  name: Medplum OAuth2 (SMART App Launch 2.0.0)
  note: Not declared as an oauth2 securityScheme in the OpenAPI (only http basic/bearer + openIdConnect are declared there), but confirmed live at the RFC 8414 authorization-server metadata endpoint and documented at docs/auth and docs/access/smart-scopes. Full detail in scopes/medplum-scopes.yml.
  sources:
  - probed https://api.medplum.com/.well-known/oauth-authorization-server
  - https://www.medplum.com/docs/access/smart-scopes
  tokenUrl: https://api.medplum.com/oauth2/token
  type: oauth2
  userinfoUrl: https://api.medplum.com/oauth2/userinfo
slug: medplum-authentication
source_filename: medplum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/medplum-fhir-api-openapi.yml\ndocs: https://www.medplum.com/docs/auth\nsummary:\n  types:\n  - http\n  - openIdConnect\n  - oauth2 (SMART App Launch 2.0.0, not declared in OpenAPI securitySchemes)\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/medplum-fhir-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/medplum-fhir-api-openapi.yml\n- name: OpenID\n  type: openIdConnect\n  openIdConnectUrl: https://api.medplum.com/.well-known/openid-configuration\n  sources:\n  - openapi/medplum-fhir-api-openapi.yml\n- name: Medplum OAuth2 (SMART App Launch 2.0.0)\n  type: oauth2\n  note: >-\n    Not declared as an oauth2 securityScheme in the OpenAPI (only http basic/bearer +\n    openIdConnect are declared there), but confirmed live at the RFC 8414\
  \ authorization-server\n    metadata endpoint and documented at docs/auth and docs/access/smart-scopes. Full detail in\n    scopes/medplum-scopes.yml.\n  authorizationUrl: https://api.medplum.com/oauth2/authorize\n  tokenUrl: https://api.medplum.com/oauth2/token\n  userinfoUrl: https://api.medplum.com/oauth2/userinfo\n  sources:\n  - probed https://api.medplum.com/.well-known/oauth-authorization-server\n  - https://www.medplum.com/docs/access/smart-scopes\nx-evidence:\n  well_known:\n  - path: /.well-known/openid-configuration\n    host: api.medplum.com\n    status: 200\n    file: well-known/medplum-openid-configuration.json\n  - path: /.well-known/oauth-authorization-server\n    host: api.medplum.com\n    status: 200\n    file: well-known/medplum-oauth-authorization-server.json\n  - path: /.well-known/oauth-protected-resource\n    host: api.medplum.com\n    status: 200\n    file: well-known/medplum-oauth-protected-resource.json\n  fetched: '2026-08-14'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medplum/refs/heads/main/authentication/medplum-authentication.yml
summary_line: http/openIdConnect/oauth2 (SMART App Launch 2.0.0, not declared in OpenAPI securitySchemes) · 4 schemes
tags:
- Healthcare
- FHIR
- Open Source
- Developer Platform
- HIPAA
- SMART on FHIR
- Clinical
- Interoperability
---
