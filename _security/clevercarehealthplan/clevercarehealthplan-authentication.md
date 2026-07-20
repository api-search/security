---
api_key_in: []
api_specs:
- filename: clevercarehealthplan-fhir-openapi.yml
  format: yaml
  label: Clever Care Health Plan FHIR R4 API
  slug: clever-care-health-plan-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevercarehealthplan/refs/heads/main/openapi/clevercarehealthplan-fhir-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Clevercarehealthplan Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Clever Care Health Plan secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Clever Care Health Plan
provider_slug: clevercarehealthplan
scheme_count: 1
schemes:
- description: SMART-on-FHIR OAuth 2.0 (PKCE S256), OpenID Connect enabled.
  flows:
  - authorizationUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/token
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/token
  name: smartOnFhir
  sources:
  - openapi/clevercarehealthplan-fhir-openapi.yml
  type: oauth2
slug: clevercarehealthplan-authentication
source_filename: clevercarehealthplan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/clevercarehealthplan-fhir-openapi.yml\ndocs: https://clevercarehealthplan.com/fhir-api-developer-resources/\nnotes: >-\n  SMART-on-FHIR OAuth 2.0 with OpenID Connect, confirmed from the server\n  /.well-known/smart-configuration and FHIR CapabilityStatement security.service\n  (SMART-on-FHIR). PKCE S256 supported; token_endpoint_auth_methods\n  client_secret_basic and client_secret_post; grant types authorization_code\n  and client_credentials. Provider Directory and Drug Formulary resources are\n  public (rate limited); Patient Access resources require OAuth 2.0.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: smartOnFhir\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/authorize\n    tokenUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/token\n    scopes: 4\n  -\
  \ flow: clientCredentials\n    tokenUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/token\n    scopes: 2\n  description: SMART-on-FHIR OAuth 2.0 (PKCE S256), OpenID Connect enabled.\n  sources:\n  - openapi/clevercarehealthplan-fhir-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clevercarehealthplan/refs/heads/main/authentication/clevercarehealthplan-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Healthcare
- Health Insurance
- Medicare Advantage
- FHIR
- Interoperability
- Patient Access
- Provider Directory
- Drug Formulary
---
