---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: cambio-healthcare-systems-booked-appointments-api-openapi.yml
  format: yaml
  label: Cambio Healthcare Systems Booked Appointments API
  slug: cambio-healthcare-systems-booked-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-healthcare-systems/refs/heads/main/openapi/cambio-healthcare-systems-booked-appointments-api-openapi.yml
- filename: cambio-healthcare-systems-default-api-openapi.yml
  format: yaml
  label: Cambio Healthcare Systems * API
  slug: cambio-healthcare-systems-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-healthcare-systems/refs/heads/main/openapi/cambio-healthcare-systems-default-api-openapi.yml
- filename: cambio-healthcare-systems-payment-notice-api-openapi.yml
  format: yaml
  label: Cambio Healthcare Systems Payment Notice API
  slug: cambio-healthcare-systems-payment-notice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-healthcare-systems/refs/heads/main/openapi/cambio-healthcare-systems-payment-notice-api-openapi.yml
- filename: cambio-healthcare-systems-protocol-api-openapi.yml
  format: yaml
  label: Cambio Healthcare Systems Protocol API
  slug: cambio-healthcare-systems-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-healthcare-systems/refs/heads/main/openapi/cambio-healthcare-systems-protocol-api-openapi.yml
- filename: cambio-healthcare-systems-well-known-api-openapi.yml
  format: yaml
  label: Cambio Healthcare Systems .well Known API
  slug: cambio-healthcare-systems-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cambio-healthcare-systems/refs/heads/main/openapi/cambio-healthcare-systems-well-known-api-openapi.yml
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Cambio Healthcare Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cambio Healthcare Systems secures its APIs with apiKey, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cambio Healthcare Systems
provider_slug: cambio-healthcare-systems
scheme_count: 4
schemes:
- description: Azure API Management subscription key, issued per COS product subscription and shown in the developer-portal profile as Primary/Secondary Key.
  in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  source: openapi/ (all 19 exported specs)
  type: apiKey
- description: Same APIM subscription key passed as a query parameter instead of a header.
  in: query
  name: apiKeyQuery
  parameter: subscription-key
  source: openapi/ (all 19 exported specs)
  type: apiKey
- authorization_endpoint: https://api.openservices.cambio.se/auth/realms/COS/protocol/openid-connect/auth
  description: Cambio Open Services authorization server (Keycloak realm COS). Client-id and client secret are emailed after a product subscription is approved. Access is scoped with SMART-on-FHIR style scopes.
  flows:
  - authorizationCode
  - clientCredentials
  introspection_endpoint: https://api.openservices.cambio.se/auth/realms/COS/protocol/openid-connect/token/introspect
  jwks_uri: https://api.openservices.cambio.se/auth/realms/COS/protocol/openid-connect/certs
  name: oauth2
  revocation_endpoint: https://api.openservices.cambio.se/auth/realms/COS/protocol/openid-connect/revoke
  source: https://api.openservices.cambio.se/auth/realms/COS/.well-known/openid-configuration
  token_endpoint: https://api.openservices.cambio.se/auth/realms/COS/protocol/openid-connect/token
  type: oauth2
- issuer: https://api.openservices.cambio.se/auth/realms/COS
  name: openIdConnect
  openIdConnectUrl: https://api.openservices.cambio.se/auth/realms/COS/.well-known/openid-configuration
  source: probed 2026-09-02, HTTP 200
  type: openIdConnect
slug: cambio-healthcare-systems-authentication
source_filename: cambio-healthcare-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://developer.openservices.cambio.se/getting-started\ndocs: https://developer.openservices.cambio.se/getting-started\nnote: 'Cambio Open Services requires TWO credentials on every call: an Azure API Management subscription key (the\n  \"API key\" shown in the COS portal profile, sent as Ocp-Apim-Subscription-Key or the subscription-key query parameter)\n  AND an OAuth 2.0 bearer access token issued by the Cambio Keycloak realm at https://api.openservices.cambio.se/auth/realms/COS.\n  The OpenAPI documents exported by the portal only declare the APIM subscription key; the OAuth layer is documented\n  on the Getting started page and in the OpenID Connect discovery document captured under well-known/.'\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  - query\n  oauth_grant_types:\n  - authorization_code\n  - client_credentials\n  token_endpoint_auth_methods:\n  - private_key_jwt\n\
  \  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  pkce:\n  - plain\n  - S256\n  mtls_supported: true\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: Azure API Management subscription key, issued per COS product subscription and shown in the developer-portal\n    profile as Primary/Secondary Key.\n  source: openapi/ (all 19 exported specs)\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  description: Same APIM subscription key passed as a query parameter instead of a header.\n  source: openapi/ (all 19 exported specs)\n- name: oauth2\n  type: oauth2\n  flows:\n  - authorizationCode\n  - clientCredentials\n  authorization_endpoint: https://api.openservices.cambio.se/auth/realms/COS/protocol/openid-connect/auth\n  token_endpoint: https://api.openservices.cambio.se/auth/realms/COS/protocol/openid-connect/token\n  jwks_uri: https://api.openservices.cambio.se/auth/realms/COS/protocol/openid-connect/certs\n\
  \  introspection_endpoint: https://api.openservices.cambio.se/auth/realms/COS/protocol/openid-connect/token/introspect\n  revocation_endpoint: https://api.openservices.cambio.se/auth/realms/COS/protocol/openid-connect/revoke\n  description: Cambio Open Services authorization server (Keycloak realm COS). Client-id and client secret are emailed\n    after a product subscription is approved. Access is scoped with SMART-on-FHIR style scopes.\n  source: https://api.openservices.cambio.se/auth/realms/COS/.well-known/openid-configuration\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.openservices.cambio.se/auth/realms/COS/.well-known/openid-configuration\n  issuer: https://api.openservices.cambio.se/auth/realms/COS\n  source: probed 2026-09-02, HTTP 200\nonboarding:\n  signup: https://developer.openservices.cambio.se/signup\n  steps:\n  - Sign up at the COS developer portal\n  - Subscribe to the \"Cambio Open Services\" product (approval required)\n  - Receive\
  \ client-id and client secret by email\n  - Read the API key (Primary/Secondary) from the portal profile\n  - Request an access token from the Keycloak token endpoint, then call the API with both the token and the subscription\n    key\n  approval_required: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cambio-healthcare-systems/refs/heads/main/authentication/cambio-healthcare-systems-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 4 schemes
tags:
- Healthcare
- Electronic Health Records
- EHR
- Clinical Decision Support
- FHIR
- HL7
- Interoperability
- Health IT
- Sweden
- Nordic
- Patient Data
- Medical Records
- openEHR
- SMART on FHIR
- Company
---
