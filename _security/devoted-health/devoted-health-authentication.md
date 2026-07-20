---
api_key_in: []
api_specs:
- filename: devoted-health-patient-access-openapi-original.json
  format: json
  label: Devoted Health Patient Access API
  slug: devoted-health-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devoted-health/refs/heads/main/openapi/devoted-health-patient-access-openapi-original.json
- filename: devoted-health-provider-directory-openapi-original.yml
  format: yaml
  label: Devoted Health Provider Directory & Formulary API
  slug: devoted-health-provider-directory-formulary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devoted-health/refs/heads/main/openapi/devoted-health-provider-directory-openapi-original.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Devoted Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Devoted Health secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Devoted Health
provider_slug: devoted-health
scheme_count: 2
schemes:
- applies_to:
  - openapi/devoted-health-patient-access-openapi-original.json
  evidence:
  - conformance/devoted-health-patient-access-capabilitystatement.json (rest.security.service SMART-on-FHIR)
  - well-known/devoted-health-smart-configuration.json
  flows:
  - authorizationUrl: https://login.devoted.com/authorize
    flow: authorizationCode
    tokenUrl: https://login.devoted.com/oauth/token
  name: SMART-on-FHIR OAuth2
  type: oauth2
- code_challenge_methods:
  - S256
  - plain
  endpoints:
    authorization: https://login.devoted.com/authorize
    device_authorization: https://login.devoted.com/oauth/device/code
    jwks_uri: https://login.devoted.com/.well-known/jwks.json
    registration: https://login.devoted.com/oidc/register
    revocation: https://login.devoted.com/oauth/revoke
    token: https://login.devoted.com/oauth/token
    userinfo: https://login.devoted.com/userinfo
  evidence:
  - well-known/devoted-health-openid-configuration.json
  issuer: https://login.devoted.com/
  name: OpenID Connect
  openIdConnectUrl: https://login.devoted.com/.well-known/openid-configuration
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
slug: devoted-health-authentication
source_filename: devoted-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://login.devoted.com/.well-known/openid-configuration\ndocs: https://www.devoted.com/developers/\nsummary:\n  types: [oauth2, openIdConnect]\n  authorization_framework: SMART-on-FHIR\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    Devoted Health's FHIR APIs use OAuth 2.0 / OpenID Connect with SMART-on-FHIR\n    authorization, as declared in each server's CapabilityStatement\n    (rest.security.service = SMART-on-FHIR) and the OpenID Connect discovery\n    document. The Patient Access API requires member-authorized (patient-scoped)\n    access tokens; third-party member-facing apps first register with Devoted's\n    interoperability team to obtain a Client ID and Client Secret. The OpenAPI /\n    Swagger definitions themselves do not declare securitySchemes, so this\n    profile is sourced from the OIDC discovery document and CapabilityStatement.\nschemes:\n- name: SMART-on-FHIR OAuth2\n  type: oauth2\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://login.devoted.com/authorize\n    tokenUrl: https://login.devoted.com/oauth/token\n  applies_to:\n  - openapi/devoted-health-patient-access-openapi-original.json\n  evidence:\n  - conformance/devoted-health-patient-access-capabilitystatement.json (rest.security.service SMART-on-FHIR)\n  - well-known/devoted-health-smart-configuration.json\n- name: OpenID Connect\n  type: openIdConnect\n  openIdConnectUrl: https://login.devoted.com/.well-known/openid-configuration\n  issuer: https://login.devoted.com/\n  endpoints:\n    authorization: https://login.devoted.com/authorize\n    token: https://login.devoted.com/oauth/token\n    userinfo: https://login.devoted.com/userinfo\n    jwks_uri: https://login.devoted.com/.well-known/jwks.json\n    registration: https://login.devoted.com/oidc/register\n    revocation: https://login.devoted.com/oauth/revoke\n    device_authorization: https://login.devoted.com/oauth/device/code\n  token_endpoint_auth_methods:\
  \ [client_secret_basic, client_secret_post, private_key_jwt, none]\n  code_challenge_methods: [S256, plain]\n  evidence:\n  - well-known/devoted-health-openid-configuration.json\napp_registration:\n  process: >-\n    Third-party member-facing applications register their organization and app\n    via Devoted's App Registration Form; Client ID and Client Secret are issued\n    by the interoperability team after review, delivered by secure (Virtru) email.\n  form: https://forms.gle/UFYvckiAeEjWP49K9\n  contact: interop@devoted.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devoted-health/refs/heads/main/authentication/devoted-health-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
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
- CMS
- HL7
- SMART on FHIR
---
