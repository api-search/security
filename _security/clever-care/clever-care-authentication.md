---
api_key_in: []
api_specs:
- filename: clever-care-coverage-openapi.json
  format: json
  label: Clever Care FHIR Coverage
  slug: clever-care-fhir-coverage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-coverage-openapi.json
- filename: clever-care-endpoint-openapi.json
  format: json
  label: Clever Care FHIR Endpoint
  slug: clever-care-fhir-endpoint
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-endpoint-openapi.json
- filename: clever-care-explanation-of-benefit-openapi.json
  format: json
  label: Clever Care FHIR ExplanationOfBenefit
  slug: clever-care-fhir-explanationofbenefit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-explanation-of-benefit-openapi.json
- filename: clever-care-healthcare-service-openapi.json
  format: json
  label: Clever Care FHIR HealthcareService
  slug: clever-care-fhir-healthcareservice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-healthcare-service-openapi.json
- filename: clever-care-insurance-plan-openapi.json
  format: json
  label: Clever Care FHIR InsurancePlan
  slug: clever-care-fhir-insuranceplan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-insurance-plan-openapi.json
- filename: clever-care-list-openapi.json
  format: json
  label: Clever Care FHIR List
  slug: clever-care-fhir-list
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-list-openapi.json
- filename: clever-care-location-openapi.json
  format: json
  label: Clever Care FHIR Location
  slug: clever-care-fhir-location
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-location-openapi.json
- filename: clever-care-medication-knowledge-openapi.json
  format: json
  label: Clever Care FHIR MedicationKnowledge
  slug: clever-care-fhir-medicationknowledge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-medication-knowledge-openapi.json
- filename: clever-care-organization-openapi.json
  format: json
  label: Clever Care FHIR Organization
  slug: clever-care-fhir-organization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-organization-openapi.json
- filename: clever-care-organization-affiliation-openapi.json
  format: json
  label: Clever Care FHIR OrganizationAffiliation
  slug: clever-care-fhir-organizationaffiliation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-organization-affiliation-openapi.json
- filename: clever-care-patient-openapi.json
  format: json
  label: Clever Care FHIR Patient
  slug: clever-care-fhir-patient
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-patient-openapi.json
- filename: clever-care-practitioner-openapi.json
  format: json
  label: Clever Care FHIR Practitioner
  slug: clever-care-fhir-practitioner
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-practitioner-openapi.json
- filename: clever-care-practitioner-role-openapi.json
  format: json
  label: Clever Care FHIR PractitionerRole
  slug: clever-care-fhir-practitionerrole
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-practitioner-role-openapi.json
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Clever Care Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
- client_credentials
overview: Clever Care secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code and client_credentials flow(s).
provider_name: Clever Care
provider_slug: clever-care
scheme_count: 3
schemes:
- applies_to:
  - Patient
  - ExplanationOfBenefit
  - Coverage
  flows:
  - authorizationUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/authorize
    flow: authorization_code
    pkce: S256
    tokenUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/token
  - flow: client_credentials
    tokenUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/token
  jwksUri: https://fhir-portal.clevercarehealthplan.com/oauth2/jwks
  name: SMART on FHIR
  revocationUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/revoke
  scopes_ref: scopes/clever-care-scopes.yml
  type: oauth2
- applies_to:
  - Patient
  - ExplanationOfBenefit
  - Coverage
  discovery: https://fhir.clevercarehealthplan.com/r4/.well-known/smart-configuration
  name: OpenID Connect
  type: openIdConnect
- applies_to:
  - Organization
  - OrganizationAffiliation
  - Practitioner
  - PractitionerRole
  - Endpoint
  - HealthcareService
  - InsurancePlan
  - Location
  - MedicationKnowledge
  - List
  name: Developer application (public resources)
  note: Public Provider Directory + Drug Formulary resources; rate-limited, require a registered app key.
  registration: https://fhir-portal.clevercarehealthplan.com/devportal
  type: oauth2
slug: clever-care-authentication
source_filename: clever-care-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi securityDefinitions + published SMART configuration\ndocs: https://clevercarehealthplan.com/fhir-api-developer-resources/\nsmart_configuration: well-known/clever-care-smart-configuration.json\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorization_code, client_credentials]\n  standard: SMART App Launch (SMART on FHIR)\n  gateway: WSO2 API Manager\nnote: >-\n  Clever Care's HL7 FHIR R4 APIs are split into two access tiers. Secured\n  Patient Access resources (Patient, ExplanationOfBenefit, Coverage) require\n  SMART on FHIR OAuth 2.0 / OpenID Connect authorization. Public,\n  rate-limited Provider Directory and Drug Formulary resources are read\n  without member authorization but require a registered developer\n  application (client credentials) obtained from the developer portal.\nschemes:\n- name: SMART on FHIR\n  type: oauth2\n  applies_to: [Patient, ExplanationOfBenefit, Coverage]\n  flows:\n\
  \  - flow: authorization_code\n    authorizationUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/authorize\n    tokenUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/token\n    pkce: S256\n  - flow: client_credentials\n    tokenUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/token\n  jwksUri: https://fhir-portal.clevercarehealthplan.com/oauth2/jwks\n  revocationUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/revoke\n  scopes_ref: scopes/clever-care-scopes.yml\n- name: OpenID Connect\n  type: openIdConnect\n  discovery: https://fhir.clevercarehealthplan.com/r4/.well-known/smart-configuration\n  applies_to: [Patient, ExplanationOfBenefit, Coverage]\n- name: Developer application (public resources)\n  type: oauth2\n  applies_to:\n  - Organization\n  - OrganizationAffiliation\n  - Practitioner\n  - PractitionerRole\n  - Endpoint\n  - HealthcareService\n  - InsurancePlan\n  - Location\n  - MedicationKnowledge\n  - List\n  registration: https://fhir-portal.clevercarehealthplan.com/devportal\n\
  \  note: Public Provider Directory + Drug Formulary resources; rate-limited, require a registered app key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/authentication/clever-care-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Company
- Life Sciences
- Health Insurance
- Medicare Advantage
- Healthcare
- FHIR
- Healthcare Interoperability
- Patient Access
- Provider Directory
- CMS-9115-F
---
