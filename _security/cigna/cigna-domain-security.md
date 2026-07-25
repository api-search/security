---
api_specs:
- filename: cigna-bulk-data-api-openapi.yml
  format: yaml
  label: Cigna Bulk Data API
  slug: cigna-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-bulk-data-api-openapi.yml
- filename: cigna-condition-api-openapi.yml
  format: yaml
  label: Cigna Condition API
  slug: cigna-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-condition-api-openapi.yml
- filename: cigna-coverage-api-openapi.yml
  format: yaml
  label: Cigna Coverage API
  slug: cigna-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-coverage-api-openapi.yml
- filename: cigna-encounter-api-openapi.yml
  format: yaml
  label: Cigna Encounter API
  slug: cigna-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-encounter-api-openapi.yml
- filename: cigna-explanationofbenefit-api-openapi.yml
  format: yaml
  label: Cigna ExplanationOfBenefit API
  slug: cigna-explanationofbenefit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-explanationofbenefit-api-openapi.yml
- filename: cigna-healthcareservice-api-openapi.yml
  format: yaml
  label: Cigna HealthcareService API
  slug: cigna-healthcareservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-healthcareservice-api-openapi.yml
- filename: cigna-insuranceplan-api-openapi.yml
  format: yaml
  label: Cigna InsurancePlan API
  slug: cigna-insuranceplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-insuranceplan-api-openapi.yml
- filename: cigna-location-api-openapi.yml
  format: yaml
  label: Cigna Location API
  slug: cigna-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-location-api-openapi.yml
- filename: cigna-medicationknowledge-api-openapi.yml
  format: yaml
  label: Cigna MedicationKnowledge API
  slug: cigna-medicationknowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-medicationknowledge-api-openapi.yml
- filename: cigna-medicationrequest-api-openapi.yml
  format: yaml
  label: Cigna MedicationRequest API
  slug: cigna-medicationrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-medicationrequest-api-openapi.yml
- filename: cigna-observation-api-openapi.yml
  format: yaml
  label: Cigna Observation API
  slug: cigna-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-observation-api-openapi.yml
- filename: cigna-organization-api-openapi.yml
  format: yaml
  label: Cigna Organization API
  slug: cigna-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-organization-api-openapi.yml
- filename: cigna-patient-api-openapi.yml
  format: yaml
  label: Cigna Patient API
  slug: cigna-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-patient-api-openapi.yml
- filename: cigna-practitioner-api-openapi.yml
  format: yaml
  label: Cigna Practitioner API
  slug: cigna-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-practitioner-api-openapi.yml
- filename: cigna-practitionerrole-api-openapi.yml
  format: yaml
  label: Cigna PractitionerRole API
  slug: cigna-practitionerrole-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-practitionerrole-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cigna.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: www.cigna.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: developer.cigna.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: fhir.cigna.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cigna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cigna, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cigna
provider_slug: cigna
slug: cigna-domain-security
source_filename: cigna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cigna.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.cigna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fhir.cigna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cigna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/security/cigna-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- CMS Interoperability
- Da Vinci
- Drug Formulary
- FHIR
- Health Insurance
- Healthcare
- Patient Access
- Provider Directory
- SMART on FHIR
- Fortune 100
---
