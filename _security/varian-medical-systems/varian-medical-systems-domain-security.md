---
api_specs:
- filename: varian-medical-systems-allergyintolerance-api-openapi.yml
  format: yaml
  label: Varian Medical Systems AllergyIntolerance API
  slug: varian-medical-systems-allergyintolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-allergyintolerance-api-openapi.yml
- filename: varian-medical-systems-careplan-api-openapi.yml
  format: yaml
  label: Varian Medical Systems CarePlan API
  slug: varian-medical-systems-careplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-careplan-api-openapi.yml
- filename: varian-medical-systems-condition-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Condition API
  slug: varian-medical-systems-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-condition-api-openapi.yml
- filename: varian-medical-systems-diagnosticreport-api-openapi.yml
  format: yaml
  label: Varian Medical Systems DiagnosticReport API
  slug: varian-medical-systems-diagnosticreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-diagnosticreport-api-openapi.yml
- filename: varian-medical-systems-documentreference-api-openapi.yml
  format: yaml
  label: Varian Medical Systems DocumentReference API
  slug: varian-medical-systems-documentreference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-documentreference-api-openapi.yml
- filename: varian-medical-systems-goal-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Goal API
  slug: varian-medical-systems-goal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-goal-api-openapi.yml
- filename: varian-medical-systems-medicationrequest-api-openapi.yml
  format: yaml
  label: Varian Medical Systems MedicationRequest API
  slug: varian-medical-systems-medicationrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-medicationrequest-api-openapi.yml
- filename: varian-medical-systems-metadata-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Metadata API
  slug: varian-medical-systems-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-metadata-api-openapi.yml
- filename: varian-medical-systems-observation-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Observation API
  slug: varian-medical-systems-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-observation-api-openapi.yml
- filename: varian-medical-systems-patient-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Patient API
  slug: varian-medical-systems-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-patient-api-openapi.yml
- filename: varian-medical-systems-procedure-api-openapi.yml
  format: yaml
  label: Varian Medical Systems Procedure API
  slug: varian-medical-systems-procedure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-medical-systems-procedure-api-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: dynamicfhir.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: varian.com
  spf: true
hosts:
- cert_expires: Oct 15 13:02:07 2026 GMT
  host: varian.dynamicfhir.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 30 15:11:32 2026 GMT
  host: www.varian.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 15:11:32 2026 GMT
  host: cancercare.siemens-healthineers.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Varian Medical Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Varian Medical Systems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Varian Medical Systems
provider_slug: varian-medical-systems
slug: varian-medical-systems-domain-security
source_filename: varian-medical-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: varian.dynamicfhir.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 13:02:07 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: www.varian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:11:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: cancercare.siemens-healthineers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:11:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: dynamicfhir.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: false\n  dmarc: false\n- domain: varian.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/security/varian-medical-systems-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Healthcare
- Oncology
- Medical Devices
- FHIR
- Radiation Therapy
- Health IT
- Fortune 1000
---
