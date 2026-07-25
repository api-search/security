---
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
