---
api_specs:
- filename: charmhealth-allergyintolerance-api-openapi.yml
  format: yaml
  label: CharmHealth AllergyIntolerance API
  slug: charmhealth-allergyintolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-allergyintolerance-api-openapi.yml
- filename: charmhealth-appointment-api-openapi.yml
  format: yaml
  label: CharmHealth Appointment API
  slug: charmhealth-appointment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-appointment-api-openapi.yml
- filename: charmhealth-capability-api-openapi.yml
  format: yaml
  label: CharmHealth Capability API
  slug: charmhealth-capability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-capability-api-openapi.yml
- filename: charmhealth-careplan-api-openapi.yml
  format: yaml
  label: CharmHealth CarePlan API
  slug: charmhealth-careplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-careplan-api-openapi.yml
- filename: charmhealth-careteam-api-openapi.yml
  format: yaml
  label: CharmHealth CareTeam API
  slug: charmhealth-careteam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-careteam-api-openapi.yml
- filename: charmhealth-condition-api-openapi.yml
  format: yaml
  label: CharmHealth Condition API
  slug: charmhealth-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-condition-api-openapi.yml
- filename: charmhealth-documentreference-api-openapi.yml
  format: yaml
  label: CharmHealth DocumentReference API
  slug: charmhealth-documentreference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-documentreference-api-openapi.yml
- filename: charmhealth-encounter-api-openapi.yml
  format: yaml
  label: CharmHealth Encounter API
  slug: charmhealth-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-encounter-api-openapi.yml
- filename: charmhealth-immunization-api-openapi.yml
  format: yaml
  label: CharmHealth Immunization API
  slug: charmhealth-immunization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-immunization-api-openapi.yml
- filename: charmhealth-medicationrequest-api-openapi.yml
  format: yaml
  label: CharmHealth MedicationRequest API
  slug: charmhealth-medicationrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-medicationrequest-api-openapi.yml
- filename: charmhealth-observation-api-openapi.yml
  format: yaml
  label: CharmHealth Observation API
  slug: charmhealth-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-observation-api-openapi.yml
- filename: charmhealth-organization-api-openapi.yml
  format: yaml
  label: CharmHealth Organization API
  slug: charmhealth-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-organization-api-openapi.yml
- filename: charmhealth-patient-api-openapi.yml
  format: yaml
  label: CharmHealth Patient API
  slug: charmhealth-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-patient-api-openapi.yml
- filename: charmhealth-practitioner-api-openapi.yml
  format: yaml
  label: CharmHealth Practitioner API
  slug: charmhealth-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-practitioner-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: charmhealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: charmtracker.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.charmhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: ehr2.charmtracker.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Charmhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CharmHealth, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CharmHealth
provider_slug: charmhealth
slug: charmhealth-domain-security
source_filename: charmhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.charmhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: false\n- host: ehr2.charmtracker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: charmhealth.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: charmtracker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/security/charmhealth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- EHR
- EMR
- FHIR
- Healthcare
- HL7
- Patient Engagement
- Patients
- SMART on FHIR
- US Core
---
