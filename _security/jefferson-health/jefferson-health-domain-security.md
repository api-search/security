---
api_specs:
- filename: jefferson-health-allergy-intolerance-api-openapi.yml
  format: yaml
  label: Jefferson Health Allergy Intolerance API
  slug: jefferson-health-allergy-intolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-allergy-intolerance-api-openapi.yml
- filename: jefferson-health-bulk-data-api-openapi.yml
  format: yaml
  label: Jefferson Health Bulk Data API
  slug: jefferson-health-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-bulk-data-api-openapi.yml
- filename: jefferson-health-condition-api-openapi.yml
  format: yaml
  label: Jefferson Health Condition API
  slug: jefferson-health-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-condition-api-openapi.yml
- filename: jefferson-health-document-reference-api-openapi.yml
  format: yaml
  label: Jefferson Health Document Reference API
  slug: jefferson-health-document-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-document-reference-api-openapi.yml
- filename: jefferson-health-encounter-api-openapi.yml
  format: yaml
  label: Jefferson Health Encounter API
  slug: jefferson-health-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-encounter-api-openapi.yml
- filename: jefferson-health-endpoint-api-openapi.yml
  format: yaml
  label: Jefferson Health Endpoint API
  slug: jefferson-health-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-endpoint-api-openapi.yml
- filename: jefferson-health-healthcare-service-api-openapi.yml
  format: yaml
  label: Jefferson Health Healthcare Service API
  slug: jefferson-health-healthcare-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-healthcare-service-api-openapi.yml
- filename: jefferson-health-insurance-plan-api-openapi.yml
  format: yaml
  label: Jefferson Health Insurance Plan API
  slug: jefferson-health-insurance-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-insurance-plan-api-openapi.yml
- filename: jefferson-health-location-api-openapi.yml
  format: yaml
  label: Jefferson Health Location API
  slug: jefferson-health-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-location-api-openapi.yml
- filename: jefferson-health-medication-request-api-openapi.yml
  format: yaml
  label: Jefferson Health Medication Request API
  slug: jefferson-health-medication-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-medication-request-api-openapi.yml
- filename: jefferson-health-metadata-api-openapi.yml
  format: yaml
  label: Jefferson Health Metadata API
  slug: jefferson-health-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-metadata-api-openapi.yml
- filename: jefferson-health-observation-api-openapi.yml
  format: yaml
  label: Jefferson Health Observation API
  slug: jefferson-health-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-observation-api-openapi.yml
- filename: jefferson-health-organization-api-openapi.yml
  format: yaml
  label: Jefferson Health Organization API
  slug: jefferson-health-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-organization-api-openapi.yml
- filename: jefferson-health-patient-api-openapi.yml
  format: yaml
  label: Jefferson Health Patient API
  slug: jefferson-health-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-patient-api-openapi.yml
- filename: jefferson-health-practitioner-api-openapi.yml
  format: yaml
  label: Jefferson Health Practitioner API
  slug: jefferson-health-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-practitioner-api-openapi.yml
- filename: jefferson-health-practitioner-role-api-openapi.yml
  format: yaml
  label: Jefferson Health Practitioner Role API
  slug: jefferson-health-practitioner-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-practitioner-role-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jeffersonhealth.org
  spf: true
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jefferson.edu
  spf: true
hosts:
- cert_expires: Aug 28 23:59:59 2026 GMT
  host: www.jeffersonhealth.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: fhir.jefferson.edu
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: smilercdr.healthpartnersplans.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Jefferson Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jefferson Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jefferson Health
provider_slug: jefferson-health
slug: jefferson-health-domain-security
source_filename: jefferson-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jeffersonhealth.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 23:59:59 2026 GMT\n  hsts: false\n- host: fhir.jefferson.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\n- host: smilercdr.healthpartnersplans.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: jeffersonhealth.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: jefferson.edu\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/security/jefferson-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Academic Medical Center
- CARIN Blue Button
- CMS Interoperability
- Cures Act
- Da Vinci Plan-Net
- Epic
- FHIR
- HL7
- Healthcare
- Hospital System
- MyChart
- OAuth 2.0
- Patient Access
- Provider Directory
- SMART on FHIR
- US Core
- USCDI
---
