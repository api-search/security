---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aetna-endpoint-api-openapi.yml
  format: yaml
  label: Aetna Endpoint API
  slug: aetna-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-endpoint-api-openapi.yml
- filename: aetna-location-api-openapi.yml
  format: yaml
  label: Aetna Location API
  slug: aetna-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-location-api-openapi.yml
- filename: aetna-organization-api-openapi.yml
  format: yaml
  label: Aetna Organization API
  slug: aetna-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-organization-api-openapi.yml
- filename: aetna-organizationaffiliation-api-openapi.yml
  format: yaml
  label: Aetna Organization Affiliation API
  slug: aetna-organizationaffiliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-organizationaffiliation-api-openapi.yml
- filename: aetna-practitioner-api-openapi.yml
  format: yaml
  label: Aetna Practitioner API
  slug: aetna-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-practitioner-api-openapi.yml
- filename: aetna-providerdirectorydata-api-openapi.yml
  format: yaml
  label: Aetna Providerdirectorydata API
  slug: aetna-providerdirectorydata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-providerdirectorydata-api-openapi.yml
- filename: aetna-patient-access-api-openapi.yml
  format: yaml
  label: Aetna Patient Access API
  slug: aetna-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-patient-access-api-openapi.yml
- filename: aetna-provider-directory-api-openapi.yml
  format: yaml
  label: Aetna Provider Directory API
  slug: aetna-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-provider-directory-api-openapi.yml
- filename: aetna-healthcare-service-api-openapi.yml
  format: yaml
  label: Aetna Healthcare Service API
  slug: aetna-healthcare-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-healthcare-service-api-openapi.yml
- filename: aetna-insurance-plan-api-openapi.yml
  format: yaml
  label: Aetna Insurance Plan API
  slug: aetna-insurance-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-insurance-plan-api-openapi.yml
- filename: aetna-practitioner-role-api-openapi.yml
  format: yaml
  label: Aetna Practitioner Role API
  slug: aetna-practitioner-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-practitioner-role-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aetna Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Aetna secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Aetna
provider_slug: aetna
scheme_count: 2
schemes:
- flows:
  - flow: authorizationCode
    scopes: 4
  name: FHIR_Patient_Allergy_Read_AccessCode_Oauth
  sources:
  - openapi/aetna-patient-access-api-openapi.yml
  - openapi/aetna-patient-access-api-sandbox-openapi.yml
  - openapi/aetna-provider-directory-api-openapi.yml
  type: oauth2
- description: "{\n \"BuildEieHeader\" : \"Header 3.2\",\n \"SecurityTemplate\" : \"FHIROpenApp\",\n \"Backend\" : \"Non-IIB, FHIRServer APIGEE APIs, requires Mutual TLS\",\n \"Errorhandlingpolicy\": \"Transparent\"\n \"Consumer\":\"External\",\n \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n}"
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://$(catalog.url)/v3/internal/auth/oauth2/app/token
  name: FHIR_Application_Oauth
  sources:
  - openapi/aetna-provider-directory-api-openapi.yml
  type: oauth2
slug: aetna-authentication
source_filename: aetna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: openapi/aetna-*-openapi.yml (derived baseline from Aetna's 95 published Swagger documents), upgraded\n  from https://apif1.aetna.com/fhir/.well-known/smart-configuration (HTTP 200), https://vteapif1.aetna.com/fhirdemo/.well-known/smart-configuration\n  (HTTP 200), https://apif1.aetna.com/fhir/v2/patientaccess/metadata, https://apif1.aetna.com/fhir/v1/providerdirectory/metadata,\n  https://developerportal.aetna.com/managedcontent/pdfs/Token_Generation_Process-Patient_Access_APIs-Production.pdf,\n  https://developerportal.aetna.com/assets/Data/createapp.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: FHIR_Patient_Allergy_Read_AccessCode_Oauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    scopes: 4\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n  - openapi/aetna-provider-directory-api-openapi.yml\n\
  - name: FHIR_Application_Oauth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://$(catalog.url)/v3/internal/auth/oauth2/app/token\n    scopes: 2\n  description: \"{\\n \\\"BuildEieHeader\\\" : \\\"Header 3.2\\\",\\n \\\"SecurityTemplate\\\" : \\\"FHIROpenApp\\\",\\n \\\"Backend\\\"\\\n    \\ : \\\"Non-IIB, FHIRServer APIGEE APIs, requires Mutual TLS\\\",\\n \\\"Errorhandlingpolicy\\\": \\\"Transparent\\\"\\\n    \\n \\\"Consumer\\\":\\\"External\\\",\\n \\\"Mutual Auth between Consumer and APIC\\\" : \\\"Not Required\\\"\\n}\"\n  sources:\n  - openapi/aetna-provider-directory-api-openapi.yml\ndocs: https://apif1.aetna.com/fhir/.well-known/smart-configuration\nprofile: SMART App Launch 1.0.0 over OAuth 2.0 authorization code with PKCE\nendpoints:\n  production:\n    authorize: https://apif1.aetna.com/fhir/prod/v1/fhirserver_auth/oauth2/authorize\n    token: https://apif1.aetna.com/fhir/prod/v1/fhirserver_auth/oauth2/token\n    discovery: https://apif1.aetna.com/fhir/.well-known/smart-configuration\n\
  \  sandbox:\n    authorize: https://vteapif1.aetna.com/fhirdemo/v1/fhirserver_auth/oauth2/authorize\n    token: https://vteapif1.aetna.com/fhirdemo/v1/fhirserver_auth/oauth2/token\n    discovery: https://vteapif1.aetna.com/fhirdemo/.well-known/smart-configuration\n  discrepancy_note: Aetna publishes two different paths for the same endpoints. The live smart-configuration\n    documents give /fhir/prod/v1/fhirserver_auth/... ; the CapabilityStatements and Aetna's own Token Generation\n    PDF give /fhir/v1/fhirserver_auth/... . Both are recorded as served. A client should read the smart-configuration\n    at runtime rather than hard-coding either.\nclient_authentication: client_secret_basic (Client ID and Secret sent as an HTTP Basic header)\npkce:\n  required_for: public clients\n  code_challenge_methods_supported:\n  - S256\nanonymous_access:\n  available: false\n  note: 'Nothing in Aetna''s API surface is callable anonymously. Even the provider directory, which carries\n    no member\
  \ data and which several peer payers expose openly, declares oauth2 on every operation. Two things\n    ARE anonymously readable and are the only unauthenticated surface: the two FHIR CapabilityStatements at\n    /metadata and the two smart-configuration documents.'\nregistration:\n  model: portal registration, then per-application, then per-product subscription\n  portal: https://developerportal.aetna.com/\n  applicant_types:\n  - third-party developer application\n  - payer (payer-to-payer data exchange)\n  - EHR application\n  - provider system\n  - ECS Provider organization (added 2026-08-19)\n  note: A call to a product the application is not subscribed to returns 401, per Aetna's own error reference.\n    Production applications go through a review, not a purchase; the production-access mailbox is AetnaInteroperabilityProductionAccess@AETNA.com.\nidentity_assurance:\n  ial2_supported: true\n  since: '2026-06-25'\n  credential_service_providers:\n  - CLEAR\n  - ID.me\n  standard:\
  \ NIST SP 800-63A Identity Assurance Level 2\n  note: Optional. The alternative Aetna calls \"Well-Known Authentication\" uses the member's Aetna username\n    and password. IAL2 applications cannot use the Sandbox environment.\nspec_template_warning: Every published Swagger declares its oauth2 tokenUrl/authorizationUrl as the un-substituted\n  IBM API Connect template https://$(catalog.url)/... - a literal placeholder, not a URL. Any tool that generates\n  a client straight from Aetna's Swagger will emit a broken auth configuration. The endpoints block above carries\n  the real values.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/authentication/aetna-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Health Insurance
- Healthcare
- FHIR
- Patient Access
- Provider Directory
- Drug Formulary
- Prior Authorization
- CMS Interoperability
- SMART on FHIR
- CARIN Blue Button
- Da Vinci
- Payers
- Fortune 100
- CVS Health
---
