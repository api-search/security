---
api_specs:
- filename: health-gorilla-binary-api-openapi.yml
  format: yaml
  label: Health Gorilla Binary API
  slug: health-gorilla-binary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-binary-api-openapi.yml
- filename: health-gorilla-capabilitystatement-api-openapi.yml
  format: yaml
  label: Health Gorilla CapabilityStatement API
  slug: health-gorilla-capabilitystatement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-capabilitystatement-api-openapi.yml
- filename: health-gorilla-coverage-api-openapi.yml
  format: yaml
  label: Health Gorilla Coverage API
  slug: health-gorilla-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-coverage-api-openapi.yml
- filename: health-gorilla-diagnosticreport-api-openapi.yml
  format: yaml
  label: Health Gorilla DiagnosticReport API
  slug: health-gorilla-diagnosticreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-diagnosticreport-api-openapi.yml
- filename: health-gorilla-documentreference-api-openapi.yml
  format: yaml
  label: Health Gorilla DocumentReference API
  slug: health-gorilla-documentreference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-documentreference-api-openapi.yml
- filename: health-gorilla-observation-api-openapi.yml
  format: yaml
  label: Health Gorilla Observation API
  slug: health-gorilla-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-observation-api-openapi.yml
- filename: health-gorilla-patient-api-openapi.yml
  format: yaml
  label: Health Gorilla Patient API
  slug: health-gorilla-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-patient-api-openapi.yml
- filename: health-gorilla-practitioner-api-openapi.yml
  format: yaml
  label: Health Gorilla Practitioner API
  slug: health-gorilla-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-practitioner-api-openapi.yml
- filename: health-gorilla-requestgroup-api-openapi.yml
  format: yaml
  label: Health Gorilla RequestGroup API
  slug: health-gorilla-requestgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-requestgroup-api-openapi.yml
- filename: health-gorilla-servicerequest-api-openapi.yml
  format: yaml
  label: Health Gorilla ServiceRequest API
  slug: health-gorilla-servicerequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/openapi/health-gorilla-servicerequest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: healthgorilla.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: www.healthgorilla.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 20:33:21 2026 GMT
  host: developer.healthgorilla.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api.healthgorilla.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Health Gorilla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Health Gorilla, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Health Gorilla
provider_slug: health-gorilla
slug: health-gorilla-domain-security
source_filename: health-gorilla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.healthgorilla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.healthgorilla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:33:21 2026 GMT\n  hsts: null\n- host: api.healthgorilla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: healthgorilla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/health-gorilla/refs/heads/main/security/health-gorilla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Interoperability
- FHIR
- Clinical Data
- Lab Ordering
- TEFCA
- QHIN
- Health Information Exchange
- Lab Results
- Clinical Documents
- SMART on FHIR
- Patient Records
- HL7
---
