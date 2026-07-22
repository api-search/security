---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Practice Fusion Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Practice Fusion secures its APIs with oauth2, openIdConnect, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Practice Fusion
provider_slug: practice-fusion
scheme_count: 3
schemes:
- flows:
  - authorizationUrl: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/token
  - flow: clientCredentials
    tokenUrl: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/token
  - flow: refreshToken
    tokenUrl: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/token
  introspection_endpoint: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/introspect
  jwks_uri: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/.well-known/jwk
  name: SMART-on-FHIR OAuth2
  standard: SMART App Launch 2.0.0
  type: oauth2
- name: OpenID Connect
  note: sso-openid-connect capability advertised in the SMART configuration; id_token issued for the fhirUser / user identity.
  type: openIdConnect
- name: Mutual TLS (client certificate)
  note: 'The CapabilityStatement security service advertises "Certificates: SSL where client must have a certificate registered with the server" in addition to SMART-on-FHIR.'
  type: mutualTLS
slug: practice-fusion-authentication
source_filename: practice-fusion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/.well-known/smart-configuration\ndocs: https://www.practicefusion.com/fhir/api-specifications/\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS]\n  standard: SMART App Launch 2.0.0 (SMART-on-FHIR)\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  pkce: S256\n  client_authentication:\n  - client-confidential-symmetric   # shared secret\n  - client-confidential-asymmetric  # private key JWT (JWKS)\n  - client-public                   # public standalone launch with PKCE\nschemes:\n- name: SMART-on-FHIR OAuth2\n  type: oauth2\n  standard: SMART App Launch 2.0.0\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/authorize\n    tokenUrl: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/token\n\
  \  - flow: refreshToken\n    tokenUrl: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/token\n  introspection_endpoint: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/introspect\n  jwks_uri: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/.well-known/jwk\n- name: OpenID Connect\n  type: openIdConnect\n  note: >-\n    sso-openid-connect capability advertised in the SMART configuration; id_token\n    issued for the fhirUser / user identity.\n- name: Mutual TLS (client certificate)\n  type: mutualTLS\n  note: >-\n    The CapabilityStatement security service advertises \"Certificates: SSL where\n    client must have a certificate registered with the server\" in addition to\n    SMART-on-FHIR.\ncapabilities:\n- launch-ehr\n- launch-standalone\n- client-public\n- client-confidential-symmetric\n- client-confidential-asymmetric\n- sso-openid-connect\n- context-ehr-patient\n- context-ehr-encounter\n- context-standalone-patient\n- context-standalone-encounter\n\
  - permission-offline\n- permission-patient\n- permission-user\n- permission-v1\n- permission-v2\n- authorize-post\nregistration:\n  process: PDS API Partner Registration -> approval -> PDS API Portal application\n  url: https://pfpds.practicefusion.com/s/Registration\n  application_inputs: [application name, description, privacy policy, JWKS URL, redirect URLs, launch URL, requested scopes]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/practice-fusion/refs/heads/main/authentication/practice-fusion-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 3 schemes
tags:
- Company
- Healthcare
- Electronic Health Records
- EHR
- FHIR
- Interoperability
- Medical
- Health IT
- SMART on FHIR
- Clinical Data
---
