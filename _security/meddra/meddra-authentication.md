---
anonymous_access: false
api_key_in: []
api_specs:
- filename: meddra-api-openapi.yml
  format: yaml
  label: MedDRA API
  slug: meddra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Meddra Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Meddra secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Meddra
provider_slug: meddra
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://mid.meddra.org/connect/authorize
    flow: implicit
    scopes: 1
    tokenUrl: https://mid.meddra.org/connect/token
  name: oauth2
  sources:
  - openapi/meddra-api-openapi.yml
  type: oauth2
slug: meddra-authentication
source_filename: meddra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: https://mid.meddra.org/.well-known/openid-configuration\ndocs: https://www.meddra.org/meddra-apis\nnote: Derived from the harvested OpenAPI securityScheme and then upgraded from the provider's own OpenID Connect discovery\n  document at mid.meddra.org, which is the authorization server the spec names. Every operation except GET /api/status\n  requires a bearer token; /api/status is explicitly documented by the MSSO as not requiring authentication. A MedDRA\n  user ID and an active MSSO subscription are prerequisites for obtaining credentials - the detailed programmer guides\n  sit behind the subscriber login at https://www.meddra.org/private/api-info.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - implicit\n  anonymous_operations:\n  - GET /api/status\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://mid.meddra.org/connect/authorize\n    tokenUrl:\
  \ https://mid.meddra.org/connect/token\n    scopes: 1\n  sources:\n  - openapi/meddra-api-openapi.yml\nidentity_provider:\n  issuer: https://mid.meddra.org/\n  product: Duende/IdentityServer (ASP.NET)\n  discovery: https://mid.meddra.org/.well-known/openid-configuration\n  discovery_status: 200\n  jwks_uri: https://mid.meddra.org/.well-known/openid-configuration/jwks\n  authorization_endpoint: https://mid.meddra.org/connect/authorize\n  token_endpoint: https://mid.meddra.org/connect/token\n  introspection_endpoint: https://mid.meddra.org/connect/introspect\n  revocation_endpoint: https://mid.meddra.org/connect/revocation\n  device_authorization_endpoint: https://mid.meddra.org/connect/deviceauthorization\n  userinfo_endpoint: https://mid.meddra.org/connect/userinfo\n  offline_access: true\nruntime_evidence:\n- url: https://mapisbx.meddra.org/api/status\n  status: 200\n  note: anonymous; body \"API is Running\"\n- url: https://mapisbx.meddra.org/api/rel\n  status: 401\n  note: 'WWW-Authenticate:\
  \ Bearer'\n- url: https://mapisbx.meddra.org/api/lang/E\n  status: 401\n  note: 'WWW-Authenticate: Bearer'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/authentication/meddra-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Medical Terminology
- Pharmacovigilance
- Drug Safety
- Adverse Events
- Regulatory
- Clinical Trials
- Healthcare
- Life Sciences
- Standards
- Ontology
---
