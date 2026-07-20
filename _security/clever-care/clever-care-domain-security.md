---
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
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clevercarehealthplan.com
  spf: true
hosts:
- cert_expires: Oct 16 10:18:09 2026 GMT
  host: clevercarehealthplan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 17:27:58 2026 GMT
  host: fhir.clevercarehealthplan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clever Care Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clever Care, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clever Care
provider_slug: clever-care
slug: clever-care-domain-security
source_filename: clever-care-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clevercarehealthplan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 10:18:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fhir.clevercarehealthplan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 17:27:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clevercarehealthplan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clever-care/refs/heads/main/security/clever-care-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
