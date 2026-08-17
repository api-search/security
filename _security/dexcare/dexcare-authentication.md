---
api_key_in:
- header
api_specs:
- filename: dexcare-visit-service-openapi.yml
  format: yaml
  label: DexCare Visit Service API
  slug: dexcare-visit-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/openapi/dexcare-visit-service-openapi.yml
- filename: dexcare-care-options-openapi.yml
  format: yaml
  label: DexCare Care Options API
  slug: dexcare-care-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/openapi/dexcare-care-options-openapi.yml
- filename: dexcare-slots-availability-openapi.yml
  format: yaml
  label: DexCare Slots Availability API
  slug: dexcare-slots-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/openapi/dexcare-slots-availability-openapi.yml
- filename: dexcare-visit-booking-openapi.yml
  format: yaml
  label: DexCare Visit Booking API
  slug: dexcare-visit-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/openapi/dexcare-visit-booking-openapi.yml
- filename: dexcare-omni-search-openapi.yml
  format: yaml
  label: DexCare Omni Search API
  slug: dexcare-omni-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/openapi/dexcare-omni-search-openapi.yml
- filename: dexcare-provider-data-management-openapi.yml
  format: yaml
  label: DexCare Provider Data Management API
  slug: dexcare-provider-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/openapi/dexcare-provider-data-management-openapi.yml
auth_types:
- oauth2
- http
- apiKey
- none
description: ''
kind: authentication
layout: security
method: searched
name: Dexcare Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: DexCare secures its APIs with oauth2, http, apiKey, and none across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: DexCare
provider_slug: dexcare
scheme_count: 7
schemes:
- description: API key issued by DexCare to the customer for API-key-to-API-key authorization. Used by the Care Options, Slots Availability, Visit Booking and Provider Data Management services. The Slots Availability document names the specific key as API_KEY_SLOTS, indicating keys are scoped per service rather than per account.
  header: x-api-key
  in: header
  name: ApiKey
  sources:
  - openapi/dexcare-care-options-openapi.yml
  - openapi/dexcare-slots-availability-openapi.yml
  - openapi/dexcare-visit-booking-openapi.yml
  - openapi/dexcare-provider-data-management-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: Patient bearer token, format `Bearer {KEY}`. Required by createVisitV9, getEstimatedVirtualVisitWaitTime and updateAcceptTerms on the Visit Service.
  header: Authorization
  in: header
  name: PatientJWT
  scheme: bearer
  sources:
  - openapi/dexcare-visit-service-openapi.yml
  type: http
- bearerFormat: JWT
  description: Staff bearer token, format `Bearer {KEY}`. Required by visitSummaryV9. Not interchangeable with the patient token — the two are declared as separate security schemes and bound to different operations.
  header: Authorization
  in: header
  name: StaffJWT
  scheme: bearer
  sources:
  - openapi/dexcare-visit-service-openapi.yml
  type: http
- bearerFormat: JWT
  description: 'The documentation-level name for the same bearer pattern: any endpoint working with protected health information (PHI) or personally identifiable information (PII) is annotated AUTH TOKEN REQUIRED in the REST API reference and needs a JWT in the Authorization header.'
  header: Authorization
  in: header
  name: bearerJWT
  scheme: bearer
  sources:
  - https://developers.dexcarehealth.com/api/
  type: http
- description: OAuth 2.0 Authorization Code Grant used to obtain the JWT bearer token. DexCare states the flow exists so the patient or authorized caregiver knowingly consents to sharing health information. Authorization and token endpoints are supplied per health system by that system's identity provider; no global endpoint, no discovery document (all /.well-known/ probes 404 — see well-known/dexcare-well-known.yml) and no scope vocabulary are published.
  flow: authorizationCode
  name: oauth2AuthorizationCode
  scopes: {}
  sources:
  - https://developers.dexcarehealth.com/api/
  type: oauth2
- description: 'Reporting service key, sent as `Authorization: dc-token <SECRET_TOKEN>`. Used by the All Visits Report and All Providers Report endpoints. DexCare warns explicitly that this token must never live in a mobile or client-side JavaScript application. Obtained from a DexCare account manager. Rejection is a 403 with {"message":"Authorization failed: bad service token"}.'
  header: Authorization
  in: header
  name: dcTokenServiceKey
  sources:
  - https://developers.dexcarehealth.com/api/reporting
  type: apiKey
  value_prefix: 'dc-token '
- description: 'Publicly available information is served without authentication: clinic and provider directories, care-options discovery, and — confirmed in the published specifications — getAggregatedSlotsV1, getAvailabilityAndWaitTimes, getRegionAvailabilityAndWaitTimes, getModalities, getAssignmentQualifiers and the entire Omni Search surface, which declares `security: [{}]`.'
  name: public
  sources:
  - https://developers.dexcarehealth.com/api/
  - openapi/dexcare-visit-service-openapi.yml
  - openapi/dexcare-omni-search-openapi.yml
  type: none
slug: dexcare-authentication
source_filename: dexcare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: https://developers.dexcarehealth.com/api/\ndocs: https://developers.dexcarehealth.com/api/\nspecs:\n  - openapi/dexcare-visit-service-openapi.yml\n  - openapi/dexcare-care-options-openapi.yml\n  - openapi/dexcare-slots-availability-openapi.yml\n  - openapi/dexcare-visit-booking-openapi.yml\n  - openapi/dexcare-provider-data-management-openapi.yml\n  - openapi/dexcare-omni-search-openapi.yml\nsummary:\n  types: [oauth2, http, apiKey, none]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  note: >-\n    DexCare runs two distinct credential families, and which one applies depends on\n    who is calling. Server-to-server integrations (care options, slot availability,\n    booking, provider data, reporting) authenticate with an API key DexCare issues to\n    the customer; patient- and staff-facing operations that touch PHI/PII\n    authenticate with a JWT bearer token obtained through the health system's own\n    identity\
  \ provider using an OAuth 2 authorization-code flow. Public directory and\n    availability reads require no credential at all. There is no global authorization\n    server — credentials, IdP and tenant host are all provisioned per health system,\n    so a developer must go through DexCare onboarding with each system they integrate.\nschemes:\n  - name: ApiKey\n    type: apiKey\n    in: header\n    header: x-api-key\n    description: >-\n      API key issued by DexCare to the customer for API-key-to-API-key authorization.\n      Used by the Care Options, Slots Availability, Visit Booking and Provider Data\n      Management services. The Slots Availability document names the specific key as\n      API_KEY_SLOTS, indicating keys are scoped per service rather than per account.\n    sources:\n      - openapi/dexcare-care-options-openapi.yml\n      - openapi/dexcare-slots-availability-openapi.yml\n      - openapi/dexcare-visit-booking-openapi.yml\n      - openapi/dexcare-provider-data-management-openapi.yml\n\
  \  - name: PatientJWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    in: header\n    header: Authorization\n    description: >-\n      Patient bearer token, format `Bearer {KEY}`. Required by createVisitV9,\n      getEstimatedVirtualVisitWaitTime and updateAcceptTerms on the Visit Service.\n    sources: [openapi/dexcare-visit-service-openapi.yml]\n  - name: StaffJWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    in: header\n    header: Authorization\n    description: >-\n      Staff bearer token, format `Bearer {KEY}`. Required by visitSummaryV9. Not\n      interchangeable with the patient token — the two are declared as separate\n      security schemes and bound to different operations.\n    sources: [openapi/dexcare-visit-service-openapi.yml]\n  - name: bearerJWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    in: header\n    header: Authorization\n    description: >-\n      The documentation-level name for the same bearer pattern: any\
  \ endpoint working\n      with protected health information (PHI) or personally identifiable information\n      (PII) is annotated AUTH TOKEN REQUIRED in the REST API reference and needs a JWT\n      in the Authorization header.\n    sources: [https://developers.dexcarehealth.com/api/]\n  - name: oauth2AuthorizationCode\n    type: oauth2\n    flow: authorizationCode\n    scopes: {}\n    description: >-\n      OAuth 2.0 Authorization Code Grant used to obtain the JWT bearer token. DexCare\n      states the flow exists so the patient or authorized caregiver knowingly consents\n      to sharing health information. Authorization and token endpoints are supplied per\n      health system by that system's identity provider; no global endpoint, no\n      discovery document (all /.well-known/ probes 404 — see\n      well-known/dexcare-well-known.yml) and no scope vocabulary are published.\n    sources: [https://developers.dexcarehealth.com/api/]\n  - name: dcTokenServiceKey\n    type: apiKey\n\
  \    in: header\n    header: Authorization\n    value_prefix: 'dc-token '\n    description: >-\n      Reporting service key, sent as `Authorization: dc-token <SECRET_TOKEN>`. Used by\n      the All Visits Report and All Providers Report endpoints. DexCare warns\n      explicitly that this token must never live in a mobile or client-side JavaScript\n      application. Obtained from a DexCare account manager. Rejection is a 403 with\n      {\"message\":\"Authorization failed: bad service token\"}.\n    sources: [https://developers.dexcarehealth.com/api/reporting]\n  - name: public\n    type: none\n    description: >-\n      Publicly available information is served without authentication: clinic and\n      provider directories, care-options discovery, and — confirmed in the published\n      specifications — getAggregatedSlotsV1, getAvailabilityAndWaitTimes,\n      getRegionAvailabilityAndWaitTimes, getModalities, getAssignmentQualifiers and\n      the entire Omni Search surface, which declares\
  \ `security: [{}]`.\n    sources:\n      - https://developers.dexcarehealth.com/api/\n      - openapi/dexcare-visit-service-openapi.yml\n      - openapi/dexcare-omni-search-openapi.yml\ngaps:\n  - No OAuth scope vocabulary is published anywhere, so scopes/ cannot be derived.\n  - >-\n    No /.well-known/openid-configuration or /.well-known/oauth-authorization-server is\n    served on any DexCare host; every probe returned 404.\n  - >-\n    Key rotation, expiry and revocation policy is undocumented for both the x-api-key\n    and dc-token credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/authentication/dexcare-authentication.yml
summary_line: oauth2/http/apiKey/none · 7 schemes
tags:
- Company
- Healthcare
- Health IT
- Patient Access
- Scheduling
- Virtual Care
- Telehealth
- Care Navigation
- Provider Data
- Search
- SDK
---
