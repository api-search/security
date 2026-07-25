---
api_key_in: []
api_specs:
- filename: clever-care-coverage-api-openapi.yml
  format: yaml
  label: Clever Care Coverage API
  slug: clever-care-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-coverage-api-openapi.yml
- filename: clever-care-endpoint-api-openapi.yml
  format: yaml
  label: Clever Care Endpoint API
  slug: clever-care-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-endpoint-api-openapi.yml
- filename: clever-care-explanationofbenefit-api-openapi.yml
  format: yaml
  label: Clever Care ExplanationOfBenefit API
  slug: clever-care-explanationofbenefit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-explanationofbenefit-api-openapi.yml
- filename: clever-care-healthcareservice-api-openapi.yml
  format: yaml
  label: Clever Care HealthcareService API
  slug: clever-care-healthcareservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-healthcareservice-api-openapi.yml
- filename: clever-care-insuranceplan-api-openapi.yml
  format: yaml
  label: Clever Care InsurancePlan API
  slug: clever-care-insuranceplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-insuranceplan-api-openapi.yml
- filename: clever-care-list-api-openapi.yml
  format: yaml
  label: Clever Care List API
  slug: clever-care-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-list-api-openapi.yml
- filename: clever-care-location-api-openapi.yml
  format: yaml
  label: Clever Care Location API
  slug: clever-care-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-location-api-openapi.yml
- filename: clever-care-medicationknowledge-api-openapi.yml
  format: yaml
  label: Clever Care MedicationKnowledge API
  slug: clever-care-medicationknowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-medicationknowledge-api-openapi.yml
- filename: clever-care-organization-api-openapi.yml
  format: yaml
  label: Clever Care Organization API
  slug: clever-care-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-organization-api-openapi.yml
- filename: clever-care-organizationaffiliation-api-openapi.yml
  format: yaml
  label: Clever Care OrganizationAffiliation API
  slug: clever-care-organizationaffiliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-organizationaffiliation-api-openapi.yml
- filename: clever-care-patient-api-openapi.yml
  format: yaml
  label: Clever Care Patient API
  slug: clever-care-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-patient-api-openapi.yml
- filename: clever-care-practitioner-api-openapi.yml
  format: yaml
  label: Clever Care Practitioner API
  slug: clever-care-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-practitioner-api-openapi.yml
- filename: clever-care-practitionerrole-api-openapi.yml
  format: yaml
  label: Clever Care PractitionerRole API
  slug: clever-care-practitionerrole-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/openapi/clever-care-practitionerrole-api-openapi.yml
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
