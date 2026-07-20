---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ellkay Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: ELLKAY secures its APIs with oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: ELLKAY
provider_slug: ellkay
scheme_count: 3
schemes:
- applies_to:
  - LKCloud Interop API
  - LKCloud FHIR R4 API
  credentials_issued_by: ELLKAY technical project team (client_id + client_secret per organization)
  expires_in_seconds: 7199
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  note: OAuth2 scopes are NOT supported; any scope headers sent by a client are ignored. Endpoint authorization is granted per client_id / subscriber_id via ELLKAY-side API permissions.
  token_type: Bearer
  token_url: https://auth2.lkidentity.com/connect/token
  type: oauth2
- in: header
  name: SiteServiceKey
  note: Non-secret routing key issued by ELLKAY that directs the request to the correct connection/data source. Required alongside the OAuth2 Bearer token on Interop and FHIR calls.
  parameter_name: SiteServiceKey
  role: routing
  secret: false
  type: apiKey
- applies_to:
  - LKCloud Interop API
  deprecated: true
  name: SubscriberKey
  note: Subscriber-key authentication retained for backwards-compatibility only; NOT supported for FHIR. ELLKAY strongly encourages migrating to OAuth2. Slated for eventual discontinuation (no date set).
  status: legacy
  type: apiKey
slug: ellkay-authentication
source_filename: ellkay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://lkcloud-api.readme.io/docs/authentication-2\ndocs: https://lkcloud-api.readme.io/docs/authentication-2\nsummary:\n  types: [oauth2]\n  primary: oauth2\n  oauth2_flows: [clientCredentials]\n  token_transport: Authorization Bearer header\n  scopes_supported: false\n  additional_headers:\n  - SiteServiceKey\nauthorization_server:\n  issuer: https://auth2.lkidentity.com\n  token_endpoint: https://auth2.lkidentity.com/connect/token\n  authorization_endpoint: https://auth2.lkidentity.com/connect/authorize\n  introspection_endpoint: https://auth2.lkidentity.com/connect/introspect\n  revocation_endpoint: https://auth2.lkidentity.com/connect/revocation\n  openid_configuration: https://auth2.lkidentity.com/.well-known/openid-configuration\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  id_token_signing_alg_values_supported: [RS256]\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n\
  \  flow: clientCredentials\n  token_url: https://auth2.lkidentity.com/connect/token\n  grant_type: client_credentials\n  credentials_issued_by: ELLKAY technical project team (client_id + client_secret per organization)\n  token_type: Bearer\n  expires_in_seconds: 7199\n  applies_to: [LKCloud Interop API, LKCloud FHIR R4 API]\n  note: >-\n    OAuth2 scopes are NOT supported; any scope headers sent by a client are ignored.\n    Endpoint authorization is granted per client_id / subscriber_id via ELLKAY-side API permissions.\n- name: SiteServiceKey\n  type: apiKey\n  in: header\n  parameter_name: SiteServiceKey\n  role: routing\n  secret: false\n  note: >-\n    Non-secret routing key issued by ELLKAY that directs the request to the correct\n    connection/data source. Required alongside the OAuth2 Bearer token on Interop and FHIR calls.\n- name: SubscriberKey\n  type: apiKey\n  deprecated: true\n  status: legacy\n  applies_to: [LKCloud Interop API]\n  note: >-\n    Subscriber-key authentication\
  \ retained for backwards-compatibility only; NOT supported for FHIR.\n    ELLKAY strongly encourages migrating to OAuth2. Slated for eventual discontinuation (no date set).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ellkay/refs/heads/main/authentication/ellkay-authentication.yml
summary_line: oauth2 · 3 schemes
tags:
- Company
- Healthcare
- Interoperability
- FHIR
- HL7
- EHR Integration
- Health Data
- API
---
