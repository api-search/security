---
api_key_in:
- header
- query
api_specs:
- filename: sun-life-authorize-api-openapi.yml
  format: yaml
  label: Sun Life Authorize API
  slug: sun-life-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-authorize-api-openapi.yml
- filename: sun-life-callback-api-openapi.yml
  format: yaml
  label: Sun Life Callback API
  slug: sun-life-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-callback-api-openapi.yml
- filename: sun-life-coverage-api-openapi.yml
  format: yaml
  label: Sun Life Coverage API
  slug: sun-life-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-coverage-api-openapi.yml
- filename: sun-life-endpoint-api-openapi.yml
  format: yaml
  label: Sun Life Endpoint API
  slug: sun-life-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-endpoint-api-openapi.yml
- filename: sun-life-healthcareservice-api-openapi.yml
  format: yaml
  label: Sun Life Healthcare Service API
  slug: sun-life-healthcareservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-healthcareservice-api-openapi.yml
- filename: sun-life-insuranceplan-api-openapi.yml
  format: yaml
  label: Sun Life Insurance Plan API
  slug: sun-life-insuranceplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-insuranceplan-api-openapi.yml
- filename: sun-life-location-api-openapi.yml
  format: yaml
  label: Sun Life Location API
  slug: sun-life-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-location-api-openapi.yml
- filename: sun-life-metadata-api-openapi.yml
  format: yaml
  label: Sun Life Metadata API
  slug: sun-life-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-metadata-api-openapi.yml
- filename: sun-life-organization-api-openapi.yml
  format: yaml
  label: Sun Life Organization API
  slug: sun-life-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-organization-api-openapi.yml
- filename: sun-life-patient-api-openapi.yml
  format: yaml
  label: Sun Life Patient API
  slug: sun-life-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-patient-api-openapi.yml
- filename: sun-life-practitioner-api-openapi.yml
  format: yaml
  label: Sun Life Practitioner API
  slug: sun-life-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-practitioner-api-openapi.yml
- filename: sun-life-practitionerrole-api-openapi.yml
  format: yaml
  label: Sun Life Practitioner Role API
  slug: sun-life-practitionerrole-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-practitionerrole-api-openapi.yml
- filename: sun-life-relatedperson-api-openapi.yml
  format: yaml
  label: Sun Life Related Person API
  slug: sun-life-relatedperson-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-relatedperson-api-openapi.yml
- filename: sun-life-token-api-openapi.yml
  format: yaml
  label: Sun Life Token API
  slug: sun-life-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-token-api-openapi.yml
- filename: sun-life-tokenhook-api-openapi.yml
  format: yaml
  label: Sun Life Tokenhook API
  slug: sun-life-tokenhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-tokenhook-api-openapi.yml
- filename: sun-life-well-known-api-openapi.yml
  format: yaml
  label: Sun Life .well Known API
  slug: sun-life-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-well-known-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Sun Life Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Sun Life secures its APIs with oauth2, openIdConnect, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Sun Life
provider_slug: sun-life
scheme_count: 4
schemes:
- api: DentaQuest FHIR Patient Access API
  authorization_endpoint: https://api.dentaquest.com/FhirPatientAccess/v1/authorize
  capabilities:
  - launch-standalone
  - context-standalone-patient
  - permission-patient
  - permission-user
  - permission-offline
  - client-public
  - client-confidential-symmetric
  - sso-openid-connect
  - launch-ehr
  - context-ehr-patient
  - context-banner
  - context-style
  code_challenge_methods:
  - S256
  flow: authorizationCode
  grant_types:
  - authorization_code
  - client_credentials
  issuer: https://dentaquest-ciam.okta.com/oauth2/ausg07qa99xVdvh4Q4h7
  jwks_uri: https://dentaquest-ciam.okta.com/oauth2/ausg07qa99xVdvh4Q4h7/v1/keys
  name: SMART on FHIR (authorization code + PKCE)
  sources:
  - well-known/sun-life-dentaquest-smart-configuration.json
  - openapi/sun-life-dentaquest-fhir-patient-access-openapi.json
  token_endpoint: https://api.dentaquest.com/FhirPatientAccess/v1/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - private_key_jwt
  type: oauth2
- api: DentaQuest FHIR Patient Access API
  id_token_signing_alg:
  - RS256
  introspection_endpoint: https://dentaquest-ciam.okta.com/oauth2/ausg07qa99xVdvh4Q4h7/v1/introspect
  name: Okta CIAM authorization server
  openid_configuration: https://dentaquest-ciam.okta.com/oauth2/ausg07qa99xVdvh4Q4h7/.well-known/openid-configuration
  revocation_endpoint: https://dentaquest-ciam.okta.com/oauth2/ausg07qa99xVdvh4Q4h7/v1/revoke
  sources:
  - well-known/sun-life-dentaquest-okta-openid-configuration.json
  type: openIdConnect
  userinfo_endpoint: https://dentaquest-ciam.okta.com/oauth2/ausg07qa99xVdvh4Q4h7/v1/userinfo
- api: DentaQuest FHIR Provider Directory API
  in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/sun-life-dentaquest-fhir-provider-directory-openapi.json
  type: apiKey
- api: DentaQuest FHIR Provider Directory API
  in: query
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/sun-life-dentaquest-fhir-provider-directory-openapi.json
  type: apiKey
slug: sun-life-authentication
source_filename: sun-life-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://api.dentaquest.com/FhirPatientAccess/v1/.well-known/smart-configuration\ndocs: https://www.dentaquest.com/en/interoperability-api\nscope_note: Applies to the DentaQuest (Sun Life U.S.) Interoperability APIs. Sun Life itself publishes\n  no public API and therefore no public auth scheme; Sun Life Link is contracted per client and Sun Life\n  Connect / mysunlife.ca are human sign-in walls.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  profiles:\n  - SMART App Launch 1.0.0\n  - OpenID Connect Core 1.0\nschemes:\n- name: SMART on FHIR (authorization code + PKCE)\n  type: oauth2\n  flow: authorizationCode\n  api: DentaQuest FHIR Patient Access API\n  authorization_endpoint: https://api.dentaquest.com/FhirPatientAccess/v1/authorize\n  token_endpoint: https://api.dentaquest.com/FhirPatientAccess/v1/token\n\
  \  issuer: https://dentaquest-ciam.okta.com/oauth2/ausg07qa99xVdvh4Q4h7\n  jwks_uri: https://dentaquest-ciam.okta.com/oauth2/ausg07qa99xVdvh4Q4h7/v1/keys\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - private_key_jwt\n  code_challenge_methods:\n  - S256\n  grant_types:\n  - authorization_code\n  - client_credentials\n  capabilities:\n  - launch-standalone\n  - context-standalone-patient\n  - permission-patient\n  - permission-user\n  - permission-offline\n  - client-public\n  - client-confidential-symmetric\n  - sso-openid-connect\n  - launch-ehr\n  - context-ehr-patient\n  - context-banner\n  - context-style\n  sources:\n  - well-known/sun-life-dentaquest-smart-configuration.json\n  - openapi/sun-life-dentaquest-fhir-patient-access-openapi.json\n- name: Okta CIAM authorization server\n  type: openIdConnect\n  api: DentaQuest FHIR Patient Access API\n  openid_configuration: https://dentaquest-ciam.okta.com/oauth2/ausg07qa99xVdvh4Q4h7/.well-known/openid-configuration\n  userinfo_endpoint:\
  \ https://dentaquest-ciam.okta.com/oauth2/ausg07qa99xVdvh4Q4h7/v1/userinfo\n  introspection_endpoint: https://dentaquest-ciam.okta.com/oauth2/ausg07qa99xVdvh4Q4h7/v1/introspect\n  revocation_endpoint: https://dentaquest-ciam.okta.com/oauth2/ausg07qa99xVdvh4Q4h7/v1/revoke\n  id_token_signing_alg:\n  - RS256\n  sources:\n  - well-known/sun-life-dentaquest-okta-openid-configuration.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  api: DentaQuest FHIR Provider Directory API\n  sources:\n  - openapi/sun-life-dentaquest-fhir-provider-directory-openapi.json\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  api: DentaQuest FHIR Provider Directory API\n  sources:\n  - openapi/sun-life-dentaquest-fhir-provider-directory-openapi.json\nanonymous:\n- api: DentaQuest FHIR Metadata API\n  note: GET /metadata conformance statement is served without credentials on api.dentaquest.com and api.deltadentalma.com.\ncredential_issuance:\n\
  \  process: Request form, manually reviewed; production credentials returned by secure email.\n  form: https://dentaquest.logicmanager.com/incidents/?t=1241&p=215&k=F0E3BD92F157F9B73EDE82834286E7CEA4044134B39D92AC3EE7E56392194241\n  self_serve: false\n  note: No self-service key issuance. The developer portal has no anonymous sign-up; the Provider Directory\n    API requires an APIM subscription key, the Patient Access API requires a registered client_id/client_secret.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/authentication/sun-life-authentication.yml
summary_line: oauth2/openIdConnect/apiKey · 4 schemes
tags:
- Insurance
- Canada
- Life Insurance
- Health Insurance
- Employee Benefits
- Group Benefits
- Dental Insurance
- Disability
- Wealth Management
- Financial-Services
- Carrier
- FHIR
- Patient Access
- Provider Directory
- Healthcare Interoperability
- CMS-9115-F
- DentaQuest
- SMART on FHIR
- Dental Benefits
---
